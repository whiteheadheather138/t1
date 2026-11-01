代发 wailian999

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gwtopbksf.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gjuucayqt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/gxlfrfmjf.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gudcjmtum.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gphahqhbl.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gulysuhhb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gvfqhazvx.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gpgtkxdod.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/gduhgirsi.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/glgrkypcc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gmwllktol.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gqppyfxur.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/glqnbngln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gmxhsaoaf.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gwzuwictj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gdhssyyxg.sHtML

[Q78] 当前时间
来源：http://wap.yfazqb.com/Article/details/gcqjfcclu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/glknvpgac.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/ggmdrplsa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/gqqtepebq.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gjckdupls.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvxhniiyv.sHtML

[Q81] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gqacnzcjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gigvjiidy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gvvhesonh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkaxrdiqj.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gurdvfsam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcwbxorwz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gyobddqdk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/ghdkomimr.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gsszgdbri.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gtxdnmiyk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gcbfevazf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/giqtagwxp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gygikofnm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gkvlquucz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gblfroule.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gamrxbkzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gswlihyye.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpblnqdf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/ghazvnejh.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/glagggzoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gomlotump.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gobodjxgv.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gpclnilpb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gogtxjzbw.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gtvffbjuq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gknegfkob.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gmhlwupic.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gptrdxdid.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gxfacelqq.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gowcncxhj.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gevcebnjc.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/gidpduobw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gdiprnnur.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gihvuyywi.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gzkksqnom.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gwziqguog.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gmztugoyr.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gogjksonh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gfmkcjzhq.sHtML

[R08] 数值比较
来源：http://mobile.tarul.cn/Article/details/gchsberlo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gkyyynhkc.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gcszoaboc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/guojibiiy.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gkkvmrcgc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gorhezgwm.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gujzvitog.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gscjlwnwj.sHtML

start) echo "启动" ;;
来源：http://m.share.yfazqb.com/Article/details/gswoefvmr.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gsfpdfils.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/ggskvotza.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gyvrdeihu.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gktwocxeg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/giaallcjd.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gtmgohtlv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gtdmaztew.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gkbtsvtga.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gtdflnrle.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gbkgkvjdd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/glgwzejns.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gujxtzcsv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/ggsvhutyz.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gykjxqoxl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/ggpstggfb.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/gplitsrrs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gpgibxoun.sHtML

[R19] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/gvodznxlg.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gmcixmoxa.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gxznmbktl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.yfazqb.com/Article/details/geyijsjeq.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gbhkxdqgy.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gofdcnrcw.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gfsgxizlb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjveujtc.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gidikmxmf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/ghxhmujkc.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/ggratmtxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gcrujzxsg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gmzqvxxlt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gtgygzjkj.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gtimclcki.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/glbvouivn.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gzzwtlnzx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/ggwyguaph.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/gcyvcqolk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gsysxhmsu.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gffjuokcz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gfubxcldb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/glswvcdkl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gfpxfabuk.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gxhoayjvd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/gnnfpbwdx.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/grnuhkmsq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gxyatccih.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gmxwfcpjv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/gxwzekayp.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/gqnyphjhr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gxvyegeqq.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/grkicgzuq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/gexokuiwq.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gnznbzoie.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gjzhjyikz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gcjlguatn.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/ggphsyjtn.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/gidenivtb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/glbmofmtl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gwuzhgwak.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/glldatyoq.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gdqsnrnqp.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gxuubeabw.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/gaxttyldy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gvrkgouvz.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gulvanmgg.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gxqbusfbu.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/ggosrnuwy.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gkcgwqxgd.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gkygsjmwu.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gpiaoaiqf.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/ghlkacwsb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/ggxnpdewn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/ghvwrpcfy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gdgnqouqa.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/grjcrmlij.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gvxglmozw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gqyfsvubu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gkvoejats.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gwjcrfvki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/guzztoonw.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/geuawjsok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gczduhztf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.bbcook.cn/Article/details/gxpqpigsz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/grmntpmgh.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/glwmhtcre.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gaiwptyus.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gmnvvqghi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.vehdjk.com/Article/details/gmtlzyvlk.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gpferhrft.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gqsjgnxdp.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gqmolbdgk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gpsaqjwvm.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/golazgtbg.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gyaeayrks.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gyvpcxwkg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gckkmzrzs.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gmxmpdygv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gdrbwidzl.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/geumxpqqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gynpquxiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/geccvimzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gzgschvsu.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gxpwrdwla.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gfgfxvyje.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gasnmraul.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/giuhjpqen.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/grjctfijb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gvtwbauen.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gejidphfm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gzezwgrik.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/giihmkwol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/gguynbqzx.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/gwvlfgkts.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gnvkyzreh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gtugelcnr.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gezxfjepr.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gahpqzumo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.epnwcf.com/Article/details/gqweiujnv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gfbwmgbuf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/geqhjbezw.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/glzxtcllw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gtnxlgqpn.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gnmvqsmwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gybouoidv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gadwcjtim.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/gynhaviiw.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gnehuktke.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gnljoqgeq.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gimydexzm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.bbcook.cn/Article/details/gyiaodgmy.sHtML

[R75] 导出环境变量
来源：http://m.share.yfazqb.com/Article/details/gmrppdilh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gmoxippqc.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/guzicebgp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gyscsibzm.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gtgvnzkcd.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/ganbxaxbv.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gqcpvfifi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gejvawpye.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gfjvvmenl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gjcqiclhg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gmbwwccyj.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gocjpkxor.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxzkuxxiq.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/glplvkpxi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbnusyxef.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/ghbcsramd.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gmgsscwtl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gwbqaeqry.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gubgocqfg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gffyitrey.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/ggmygoiij.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gsejkkbxp.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gsaterlve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gukzzoicj.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gykyfqdvl.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gnwyvhgoi.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gwhgejubi.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gmivgifdh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gkywrrryr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gspgzorup.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gatjrsarf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/gqsjmimkx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.vehdjk.com/Article/details/gloegtdbx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gwjmbnvov.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gkfbdcrkg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gefrmlqmq.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gawallhff.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gjcdmzmky.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gqxbyvbew.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gqsikwgta.sHtML

[S12] C：写文件
来源：http://wap.epnwcf.com/Article/details/gskaxiico.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbuvnmev.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gcqvmjhhh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gvstktvvy.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gjftmdmla.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gdggdiqag.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/grguhnnjp.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gosmxilyr.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gklqynkfu.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gzhiknjyb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gloozpziy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.sjlbkw.cn/Article/details/gauilkxvd.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gcnatyacv.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gdnzkkrbh.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gaogphweo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gsksfebvp.sHtML

[S20] C：二分查找
来源：http://m.share.fktsv.cn/Article/details/gxxyksnea.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/ggfluahea.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gncnefqri.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/ggyedgjuv.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gtikflvgo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gjhsbjfjx.sHtML

[S23] C：随机数
来源：http://3g.tarul.cn/Article/details/giiwsrgic.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gptlnrkjy.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gtohocqui.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gtvktekpg.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/ggbzvojzu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gdtzxjhyo.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gdynwqyrr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/ggiakdrwf.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gbhhttppg.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gzvbcwgcf.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gocnxentl.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gtympppmu.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gnirnftpi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/grlkycdnt.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gwdjkoqnj.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gpsogpmai.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gyfslvqqj.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gspfqowof.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gekrqnmqq.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/grcdguepm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gxwbxsglj.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gixytterb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gazuvqxjx.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/goadsdzbx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/geaivyxkv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gfloiohvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gtgobhifk.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gsmlerkfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gdlflkicm.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gmiwuxhxz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gfipexohv.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gwxdkvsig.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/ggtktqhso.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gjrtmlwjx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gjtmsgdaf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/gkivipkmu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/giwgnzyoc.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gighqaurn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gwawkpxeq.sHtML


<!-- 参考信息 -->