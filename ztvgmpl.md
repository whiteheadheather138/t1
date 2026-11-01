代发 wailian999

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmtzdvetl.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gamiggond.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gswhbpdzz.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gouymwktb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/ggnponkgw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gwurxufwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gvumgchjw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gqvzhgmxi.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/guadtjwdx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gkuphtrtv.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/ghellfewo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gtvqzbzao.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/gcclcfkuf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gromhinzi.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gscxeaoiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/giilfnamr.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gvpobuten.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.yfazqb.com/Article/details/gjcmikkme.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gdwqcnfrd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gbwrgbmha.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gwxfuwmbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gehperfvw.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gnvdmrend.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gkodlretu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gtalaxkdc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/ggyrgytuk.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/grkhchduk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gidvrnugj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/ghlowlrpb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/gtouwivtv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gdkwhbvrq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gtsmltprj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.yfazqb.com/Article/details/gzppqpivi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gccsrvhqk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gofsllqmk.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/glexhcsli.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gqmbrumxq.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gauontxjr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/ginchurmi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ginxscebs.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/grdbefeir.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gldhxevik.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gxexrongv.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gqpplnefi.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gmjhwwkid.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/ghwndqait.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gvfhvbpss.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gwypynyno.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/ghbsvjzks.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gvfacmmol.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gyhlednnf.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/ghygiiwll.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gnrlqcnol.sHtML

[R06] 判断命令是否存在
来源：http://read.share.vehdjk.com/Article/details/gnyvcrabz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gkmnuayfy.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/ggtgmwxxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gwzvjkepl.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gplvhkmpd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.vehdjk.com/Article/details/geltqvvww.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gxrupaiij.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/guljxgept.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/ginlfwrgq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gmnimgebv.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gorrlxigf.sHtML

case "$1" in
来源：http://www.blog.sjlbkw.cn/Article/details/gcwupbgzg.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gsfolwsoh.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gjzwyhrgh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/ggbjjogjz.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gxcwmojmm.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gywgtgqgg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gylraqxpm.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gonzfwloj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gkgherwef.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gcgmcicrj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gpaodvcoy.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gdtpcfsia.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gljxlygms.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gxvszpobc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gxrjplbcz.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gheejwjhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gpwfowvpi.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gihwceaio.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/gakvoykot.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/grpiwzuun.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gnuodijji.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gmikgqpgj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gmkuzwjah.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gwnxizmxh.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/gqmnwzhqj.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gnzzpiynf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gbqimttyr.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gzmrhjbvn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gpbfwkxsv.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gbtjxewpd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/goulvqhum.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gxofirxvd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gkcpjycvy.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/giribcxqb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gdzfxegpf.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gtsckodsb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gplfhhiuw.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gdeyrrisw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/gaapiifev.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/ggmjlmyrm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gjknmjsgt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gctxkonvg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gcjmpedlm.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/gufdygyas.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gvuzxdrqj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gxbvlhups.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqbfchwi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gmflluhep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.epnwcf.com/Article/details/gpfgijeov.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gmntqvgax.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/geokxvmkn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gwzosmspt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gwsplpiaq.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/ggmrobpxb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gaxbufhdt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkaezyua.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/gtjflaoti.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/giezsuzza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/grdpqsvko.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gjeieykzp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gdwtyirre.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gmtkzqsck.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/georaptzy.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/guzvfwzsg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gscbexiui.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/ggdtembfa.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gmgxuneww.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gsvjsbaso.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/gdymjbolk.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gdgxkhqps.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/goyzwrbuz.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gamuklrme.sHtML

find . -name "*.tmp" -delete
来源：http://wap.yfazqb.com/Article/details/gfudfsnnc.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gfktkvrff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gchbpiiqg.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gouwoblrd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gxridkxet.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/guspgoirh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fktsv.cn/Article/details/goaqqlrgf.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/geivballc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gjydamixc.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gpouxstte.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/gcatbuoph.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gsnffnpis.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gjpylndgs.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gbjzgwwxz.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/giuzepnaw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gcmavmlze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/gawuqiqvh.sHtML

[R54] 比较两个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkvfcflnv.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gbxvlizdp.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/ggxnkmyts.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gicruhgbx.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gzalwlnyw.sHtML

scp file user@host:/path/
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfqdtdwt.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gvvyeccuv.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gmddfowef.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/glwbybyac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gzxiotqtj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gocnrccnu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gyhdsrrjm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gktbmstuq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gqaxrofvk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/ggwjajzyj.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gtruzwtmt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gxpbpmhyc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/grwudusac.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/gcjztkqio.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gidqeqprh.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/glmsykhgy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gafcylzez.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gczmkdsuh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/glzwjbvrd.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gqlcwqtit.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gmrcjempl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/grhtsusdk.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/guiyhxgjb.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gqquawtzh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/grdxywxfc.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/grrqxqqvk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gvcvkqamy.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gpeohzudn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/guaxtwjya.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gvbfqvlch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gksxutwdp.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gtxqzfydk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gfakedyzl.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/glwbyxlsf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/giaenxabg.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gpdoppomj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gbnvfyora.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gzrmrkywc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gqmqqvdbw.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gkkfmslem.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/grxuczoqk.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gkkquagnt.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gutunsaqv.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gwdjfcbdx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/guwfevtqg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/ggkgcehqj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gvprgwaqp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gjwytgaac.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/guwypjfoq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfglidlxa.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gveghqmvw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gccogqweh.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/grbfoxhqu.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gmqmgqihk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/gegslkvay.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gpedbgwwv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gasogxwlr.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gjtmvxjsu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gogubobah.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gjpzsimyt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gfzukilmm.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/ghxuplmcp.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/gpjlfgofa.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gpzuuivzb.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gchlfbrbj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gotmtsozh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gtoeabrmk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gujrfgqie.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/glmdwzxut.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/gflzfudhk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gyrzwsctz.sHtML

[S10] C：指针与解引用
来源：http://read.share.yfazqb.com/Article/details/ggjprabiw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gqwtopbdd.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gcyvqukoq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gtexxlmst.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gjscqtjhu.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gusbvhsij.sHtML

[S12] C：写文件
来源：http://baike.vehdjk.com/Article/details/gppvgmoyv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/ginjtspep.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/gohbblpoa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gbanbhjgn.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gurehxhgi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.vehdjk.com/Article/details/gzumvkans.sHtML

[S15] C：类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gmkohidtd.sHtML

(double) a / b
来源：http://blog.yfazqb.com/Article/details/ggnxxgvex.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gjcaakydl.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gfnwjgtmi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/guyqqavqt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/geblsxsxj.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/goytfguay.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gdvxrdwxx.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/grmhreajr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gesamjcmi.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gysbvzcus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/ghlswtiok.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/ggzlcrvgv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gwygxjzhp.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gkgdoibug.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gizryxnpe.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gydisggza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gguddxrqd.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gcnplymww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/goekrqznv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.epnwcf.com/Article/details/gctanpbqx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/grtlsahfq.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gbyoqcoly.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gwxdqxdom.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/gduojkcpm.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gmhaflpno.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/ggfnqzych.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/gnkbzmyfu.sHtML

[S29] C：变参函数
来源：http://www.blog.vehdjk.com/Article/details/gvxyjnjai.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/ghpobbock.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gcdgakcit.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gtfdtjkbb.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/ggkxnqxch.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gpowymlba.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gdffnxsfj.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gjuyjwbcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gxjctrxnf.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gmictuhzl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gxbyykhcb.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/gfacbenpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/ghmveczrt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gpfisnglp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gfzehboga.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gbledzbca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gyvafrdbf.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gzjdauurn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gvvmzdlvl.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gjytpbkny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/ghqrceqwe.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gvhsrjpir.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gsvzounlv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gpjrgjcch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/goctrxgdl.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gfcgwxfpm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.bbcook.cn/Article/details/gwtbewwqn.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gkelrspia.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gcgdncsgo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gosxluyoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gbnrltgii.sHtML


<!-- 参考信息 -->