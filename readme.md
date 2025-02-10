#README

We've turned off the ability to report issues directly on this repo and do not monitor PRs.

Provide feedback here: https://aka.ms/provide-feedback

Or, if you are a trainer with a microsoft.com email address, please create a ticket in AzDO.

# GitHub-Benutzerhandbuch für MCTs

Clouddienste wie Microsoft Azure werden häufig aktualisiert, was zu Herausforderungen für Microsoft Certified Trainer (MCTs) führt, wenn sie Kurse unterrichten und die Labschritte nicht mehr mit unseren Clouddiensten übereinstimmen. . Aufgrund der Häufigkeit der Änderungen und der Tatsache, dass es nicht immer eine Benachrichtigung gibt, wenn Änderungen auftreten, kann es für das Kursentwicklungsteam schwierig sein, Änderungen an den Labs schnell zu erkennen und die entsprechenden Anpassungen vorzunehmen.

Um diese Probleme zu beheben, verwenden wir GitHub, um die Labschritte und -skripts für Kurse zu veröffentlichen, die Clouddienste wie Azure behandeln. Die Verwendung von GitHub ermöglicht es den Kursautoren und MCTs, Labinhalte bei Änderungen an Clouddiensten auf dem aktuellen Stand zu halten. Mithilfe von GitHub können MCTs Feedback und Vorschläge für Änderungen an den Labs bereitstellen, und die Kursautoren können die Labschritte und Skripts umgehend aktualisieren.

Wenn Sie sich darauf vorbereiten, solche Kurse zu unterrichten, sollten Sie sicherstellen, dass Sie die aktuellen Schritte und Skripts für Labs verwenden, indem Sie die entsprechenden Dateien von GitHub herunterladen.

Dieser Leitfaden richtet sich an MCTs, die noch keine Erfahrung mit GitHub haben. Er enthält Schritte zum Herstellen einer Verbindung mit GitHub, zum Herunterladen und Drucken von Kursmaterialien sowie zum Aktualisieren der Skripts, die Lernende in Labs verwenden. Außerdem wird erläutert, wie Sie sicherstellen können, dass die Inhalte eines Kurses auf dem aktuellen Stand sind.

> **Hinweis:** Die Microsoft Learning-Unterstützung für den Zugriff auf Dateien auf GitHub und für die Navigation auf der GitHub-Website ist auf MCTs beschränkt, die diesen Kurs unterrichten.

GitHub sollte nicht verwendet werden, um technische Inhalte im Kurs zu diskutieren oder sich über die Vorbereitung auf den Kurs oder seine Labs auszutauschen. Es ist ausdrücklich für Änderungen an den Labs vorgesehen.

 
> **Hinweis:** Für allgemeine Kommentare zum Kurs und zu Demos sowie für Informationen zur Vorbereitung auf den Kurs verwenden Sie bitte die MCT-Foren.

## Abschnitte

- [GitHub-Terminologie](https://microsoftlearning.github.io/MCT-User-Guide/terminology/)

- [Empfangen von Aktualisierungsbenachrichtigungen und Zusammenarbeit an Projekten](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/)

- Vorschlagen von Änderungen oder Übermitteln eines Problems im Zusammenhang mit Labanweisungen

## GitHub-Terminologie

Für GitHub werden Begriffe eingeführt, mit denen Sie möglicherweise nicht vertraut sind. Die folgende Liste enthält Begriffe und Konzepte, die in diesem Dokument verwendet werden. Eine vollständige Liste der GitHub-Begriffe finden Sie im [GitHub-Glossar](https://docs.github.com/en/get-started/quickstart/github-glossary).

| Begriff| Erklärung |
| - | - |
| Git und GitHub| Git ist ein Open Source-Programm zur Änderungsverfolgung, und GitHub ist eine auf Git basierende Website/Lösung. Es gibt andere Websites und Lösungen, die Git als Back-End verwenden. GitHub wird hauptsächlich für Open-Source-Entwicklungsprojekte (öffentliche Projekte) verwendet und ist für diese Projekte kostenlos. Wenn Sie jedoch GitHub für Projekte verwenden möchten, die privat und nicht Open Source sind, müssen Sie sich für eine kostenpflichtige Version registrieren. |
| Repo oder Repository| Jedes Projekt in GitHub befindet sich in einem Repository oder Repo. Ein Repository enthält alle Dateien für ein Projekt, einschließlich Dokumentation, und unterstützt den Revisionsverlauf. Ein Repository kann öffentlich oder privat sein. Sie können eine lokale Kopie des Repositorys auf der Festplatte Ihres Computers speichern oder das Repository in GitHub verwenden. |
| Markdown| Dies ist ein Textdateiformat, das zum Erstellen von Dokumentationen verwendet werden kann. Es ist textbasiert und sehr einfach zu aktualisieren, was die Zusammenarbeit erleichtert. GitHub rendert den Text dann als HTML. |
| GitHub Flavored Markdown (GFM)| Es gibt viele Variationen („Flavors“) des Markdowndateiformats. Die GitHub-Version, die häufig als GFM bezeichnet wird, ist eine der häufigsten Markdownvarianten. Weitere Informationen zu GFM und zur Verwendung des Markupformats für Ihre GFM-Dokumente finden Sie im Artikel „Erste Schritte beim Schreiben und Formatieren auf GitHub“ unter https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github/. |
| Fork| Dabei handelt es sich um eine Kopie eines anderen Repositorys, die sich in Ihrem GitHub-Konto befindet. Dies unterscheidet sich von einem Branch, der sich im ursprünglichen Repository befindet. Siehe „Branch“ weiter unten. |
| Verzweigung| Dies ist eine Kopie eines Repositorys, die sich im selben Repository wie das Original befindet. Sie können einen Branch mit dem Original zusammenführen. |
| Abrufen| Dies ist der Vorgang zum Abrufen einer Kopie der letzten Änderungen aus einem Onlinerepository. Bei einem Abruf werden allerdings keine Änderungen zusammengeführt. |
| Pull| Dies ist der Prozess des Abrufens der letzten Änderungen aus einem Onlinerepository, wobei die Änderungen mit lokalen Änderungen zusammengeführt werden. |
| Merge| Dies ist der Prozess zum Abrufen von Änderungen aus einem Branch, die dann auf einen anderen Branch angewendet werden. Dazu gehört auch das Abrufen von Änderungen aus einem Onlinerepository und das Anwenden dieser Änderungen auf die lokale Version des Repositorys. |
| Pull Request| Dies ist eine Gruppe von vorgeschlagenen Änderungen an einem Repository, die ein Benutzer übermittelt. Die Besitzer oder Projektmitarbeiter können Pull Requests dann annehmen oder ablehnen. |
| Push| Dies ist der Prozess des Sendens oder Einreichens Ihrer lokalen Änderungen an einem Onlinerepository. |
| Projektmitarbeiter| Dies ist ein GitHub-Benutzer, der über Berechtigungen zum Hinzufügen, Löschen oder Ändern des Inhalts eines Repositorys verfügt. |

## Empfangen von Aktualisierungsbenachrichtigungen, Vorschlagen von Änderungen und Zusammenarbeit an Projekten

Sie können GitHub so konfigurieren, dass Sie Benachrichtigungen erhalten, wenn Aktualisierungen an einem GitHub-Repository vorgenommen werden. Es gibt mehrere Möglichkeiten, wie Sie Benachrichtigungen abonnieren können. Viele davon hängen mit den unterschiedlichen Verfahren zusammen, wie Sie an einem Projekt zusammenarbeiten können. Zum Empfangen von Benachrichtigungen können Sie die folgenden Aktionen ausführen.

| Aktion| Beschreibung |
| - | - |
| [Überwachen von Repositorys](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/watching/)| Wenn Sie ein Repository überwachen, abonniert GitHub automatisch Benachrichtigungen für neue Pull Requests oder Issues, die für dieses Repository erstellt werden. Sie überwachen automatisch jedes Repository, das Sie erstellen oder bei dem Sie Projektmitarbeiter sind. |
| [Pull Request](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/pullrequest/)| Wenn Sie einen Pull Request erstellen und vorschlagen, dass die Besitzer eines Repositorys eine von Ihnen vorgenommene Änderung annehmen, abonnieren Sie automatisch Benachrichtigungen für die zugehörige Unterhaltung über den Pull Request. Um einen Pull Request zu erstellen, müssen Sie zuerst einen Branch erstellen. |
| [Kommentare](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/comment/)| Wenn Sie Kommentare zum Pull Request einer anderen Person abgeben, abonnieren Sie automatisch in GitHub das Forum für diesen Kommentar, oder Sie können das Forum manuell abonnieren. |
| [Probleme](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/issue/)| Ein Issue ist ein Vorschlag, eine Frage oder eine Anforderung, die sich auf ein Repository bezieht. Zu jedem Issue gehört eine eigene Unterhaltung. Sie können Issues abonnieren, oder GitHub abonniert automatisch Issues für Sie, die Sie erstellen. |
| [Erwähnungen](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/mention/)| Wenn ein anderer Benutzer Sie in einer Unterhaltung erwähnt, indem er Ihren GitHub-Benutzernamen ([@username](https://github.com/username)) verwendet, abonniert GitHub die Unterhaltung automatisch. |

> **Hinweis:** Sie können ändern, wie und wann Sie Benachrichtigungen erhalten, und Sie können auch Abonnements für einzelne oder alle Unterhaltungen beenden.

## Übermitteln von Issues oder Vorschlagen von Änderungen an Labanweisungen

Wenn Sie einen Vorschlag machen möchten oder einen Fehler in einem Lab bemerken, können Sie entweder einen Pull Request senden und ein Issue protokollieren. Wenn Sie die Lösung für den Fehler bereits kennen, sollten Sie einen Pull Request senden. andernfalls übermitteln Sie ein Issue.

| Aktion| Beschreibung |
| - | - |
| [Pull Request](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/pullrequest/)| Wenn Sie einen Pull Request erstellen und vorschlagen, dass die Besitzer eines Repositorys eine von Ihnen vorgenommene Änderung annehmen, abonnieren Sie automatisch Benachrichtigungen für die zugehörige Unterhaltung über den Pull Request. Um einen Pull Request zu erstellen, müssen Sie zuerst einen Branch erstellen. |
| [Kommentare](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/comment/)| Wenn Sie Kommentare zum Pull Request einer anderen Person senden, abonnieren Sie automatisch in GitHub das Forum für diesen Kommentar, oder Sie können das Forum manuell abonnieren. |
| [Probleme](https://microsoftlearning.github.io/MCT-User-Guide/collaboration/issue/)| Ein Issue ist ein Vorschlag, eine Frage oder eine Anforderung, die sich auf ein Repository bezieht. Zu jedem Issue gehört eine eigene Diskussion. Sie können Issues abonnieren, oder GitHub abonniert automatisch Issues, die Sie erstellen. |
