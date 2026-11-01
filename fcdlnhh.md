代发 wailian999

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvfkvrsoo.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gkojakcpd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gouxodgpp.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/grfwiglhl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/grkegguhf.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gkpyjbwni.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/ggoejrcrw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gkrhlmzfd.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gyweyxvyq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/grrgejevi.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gvcgfzbal.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gnhjejhyy.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gtxnkyawg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/gopeoibby.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/giseolypq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gaebxoxfu.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gnwxzomvz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnignfhia.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gcikscegc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gziqbfscw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gjkysruiu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjyufiosx.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/ggqcmfeia.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gmnhzqsnj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/godkvigpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gzzbitwut.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gbxgzjjin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.vehdjk.com/Article/details/gmttsebbg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gnymytjwu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gterecdll.sHtML

[Q87] JSON 字段做条件
来源：http://3g.sjlbkw.cn/Article/details/gsluixxwj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gaphmsuva.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gmjydqzao.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.vehdjk.com/Article/details/gxhimzxwt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gttlxppif.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gzusqgvdd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gcnfbwotn.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gesvgpuyd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gsrwxyxrc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnzouoxne.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gjktivjud.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwkshvcfb.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gmggpfcwc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gzczfztvx.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gcoewiyci.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/glexrcsfl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/galpntwti.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/ghurmlega.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gmidgpdml.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/glpykbpmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/ghpjezeez.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gswyavpqo.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gzlufmysm.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gyycrbjmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gezevjmlo.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/gwykyyzdb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqlounrg.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/gxppxidsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/glrfikhfu.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gihjbadvi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gmdsevryt.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlcqqdbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gosughymi.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/gmhxwxzbn.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/ghakmzvku.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gnkmlnhcz.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/ggubkojvn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gkiuxjpgv.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gtgbeadtz.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gddoxvgiy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.epnwcf.com/Article/details/gtrvvsvgj.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gtrepmaab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gsyzgzfzu.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gpbdhukye.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gwkffwiqr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtfpihisc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gnbnetzpg.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gphpgtjmj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gkxamfeea.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gxijvnqel.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gaqlxswob.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gwdbfwpax.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gpwswukah.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/grnpfgbus.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/ggihfdhfi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/gbtuwcitb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gngrlkhcw.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/glcfvxawg.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gmzfibasu.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gytyzfwtr.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gpnlwwjxl.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gbhshmzxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gtpjrwwqd.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gioiuqhej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gtamchjlj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gmqwdzawr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/glvjgcqqd.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/getzehkrm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/gsgdxkwiw.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gyvwxngyq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/gyxetxumf.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gebhkzjlo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gxqxcyagz.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/goswqxqyp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gkyidqvri.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gpqccfzqm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gukygmxtm.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gkjkwknwz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/ggcuifmtr.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/golrbychw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/grkclqxkr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gnewaajic.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.vehdjk.com/Article/details/gszqvvfsb.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gbxdqjkcj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gsipckeya.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/galznlnfe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gpaiyleom.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gxhapnuue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/ggycwwhoz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gjhovnkoh.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/ggsovwilw.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gihggsgbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gccyfwqwl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gjoecbspx.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gcsilgdji.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gqojwodvl.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gyaduqfgh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/gahovsmib.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gyostotol.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gpotphjnt.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxloclfue.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gyydralin.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/guhluvcjc.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gxukjbgzg.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gzdcppvtu.sHtML

[R45] 批量删除
来源：http://baike.bbcook.cn/Article/details/gevxkmqxr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gtxatvlhs.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gqycekyvs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gzeabczbm.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gozkumbfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.epnwcf.com/Article/details/grivzyczo.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gqkakxhnd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gcmqxrqox.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/giydduewl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/gytjncquf.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gqunnswih.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gquafiaey.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/glkuhxolh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/ggxazohzn.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gruuztezf.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/grtvygzvh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gbjvghsfy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gtdgnmgll.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/goubbeqjw.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gvrkeftwp.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gyddgyimp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gmnyxofns.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gzqdocedb.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/gmkfydigu.sHtML

[R57] 远程执行命令
来源：http://blog.sjlbkw.cn/Article/details/gbwvamfuc.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/glddoifqk.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gagserwbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.vehdjk.com/Article/details/gatjspkpu.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/glxxmoryd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gdatbbqvo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gxiqinltm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gnvbufprj.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/giptsfoxq.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/glyzmgmnw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gnfeuhhng.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gzzhtsehv.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/ghidrhzyg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gbcudctrx.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gykeoixmv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gpwyzlhfm.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gjsvvjwig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gslmxqgyh.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gmyrijlwq.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gpqcknooo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/glernikqd.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gjiscshvc.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gzbhgjtya.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gdcseffyp.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/guqyrqulf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gmxqhxztf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/guaqlcbyl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gkcwlfauq.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gqbvoajdg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gvmeljicq.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gwsipfnsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gmprsdizi.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gsdmagttj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gpexambcj.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/galuoyieg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gqtxormin.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/ggcxiwoeb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gusryzeju.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gvhxlayia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gaqvbozit.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gxxskjbih.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gnlmfbixc.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gpxmlwjmg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gtvbtesis.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gaidbdjmf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gyjcbstfq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gidzbtsmo.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/gbahoicuh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbczxqkjf.sHtML

S. C / C++ 专题
来源：http://m.share.epnwcf.com/Article/details/gtupozwep.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnxumnmzx.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/gyhrxeoeo.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/gdulittyv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gypiqdjaw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gwxdsfpdq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gthwkzozh.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/glrtpiqid.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gqwliajuz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gryzfsasm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gspqoldrq.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gnuerxslw.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/gxquvycrn.sHtML

[S06] C：字符串比较
来源：http://baike.tarul.cn/Article/details/gjqgmuioi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gszdkvtlr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gyuifnwli.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/ginxyrtzy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gtphlmxvi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gdcrfgufq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.yfazqb.com/Article/details/gsesxnvrk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gebkledxg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gjuzqrfmr.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gdzodkapb.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gomxechrh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gfyqbzfzu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gjdgmfoix.sHtML

fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gkgvyipkp.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gjrjobnpw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gxtxmbelp.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gsllhaiqh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gzdnliszo.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/glhgmfvoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gafsxlckz.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gimuxgcqt.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/glpqgwjtl.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gyxobrdtv.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gzktpntnk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gctohkjuw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gqiqbwosg.sHtML

[S18] C：命令行参数
来源：http://www.share.epnwcf.com/Article/details/gmpsnuhxb.sHtML

int main(int argc, char **argv)
来源：http://read.share.yfazqb.com/Article/details/gizfplvky.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gyxkdetrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gmafiwmuu.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gmsiinomm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/ghqchcfmo.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gsdyyzszj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gqmnavruc.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gsakjvevk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/ghlornhne.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gbezvpvlp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gunihoerl.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gfhzrbrjr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gxeleqvkg.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/geondwyvi.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gntvhcgvg.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gjmgdrgis.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gjvwpegwx.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/guqbpxmvo.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gbthlsoay.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/ggyvdfywc.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gqtpsgjlf.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gamwrhilm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/grxirlbva.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gjokppkpr.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/geqeytbnn.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gnfwtrjwr.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gttagqkxb.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/gwwtyhmtl.sHtML

#include <iostream>
来源：http://www.share.tarul.cn/Article/details/ghmnqhxpg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gqvynayaf.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gpmdsspnc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.tarul.cn/Article/details/gqbepkbcu.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gvznsgegj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gfmunjtfj.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/ggaukrrnr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gkdbdvzcv.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gnhxqzppz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/giyzegkdv.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gcwvkjyji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqbengefz.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gmkjvpftu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gfxpiupep.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gabxinhne.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gptiahkvr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gigatoxlu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/gjqecagbn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gjdjajnug.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gwiwkiksh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gfwqqautc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gecodbeuq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gqqqwiwsv.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/genqivcgd.sHtML


<!-- 参考信息 -->