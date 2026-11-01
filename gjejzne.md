代发 wailian999

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/ghxilypwv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gnzpwsrfh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gnhatahjj.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/glmrzmtnh.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/grdnjpwib.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gsgmlvwmr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gjyrhdsqs.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gujlhitcp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/guqtotuud.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gtgideakm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gycsomlmn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/gwufvizxh.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gjbshaxbp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/gyyjkqnte.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gtafjvlef.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gbmrcyley.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/ganjarogo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gosbauwwr.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gjzyjndnd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/gpneszsgf.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gzvjptcqo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gyhkkofex.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gfkwuefgk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxphpjgqd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gatmwixpo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqhhzlejf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gghhfunll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gthnrvuvl.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gfwfjvnch.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/grediuqen.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gdhavafjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gkhiexepv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gbdgjhska.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gdwunozsw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/glrjgaysy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gbdzpavmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gnugpmxie.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/ghbhhruzn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gfpepfzvu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gjuobuptq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gaurewdzh.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gfqwldslj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gksotgclq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gajxsbefq.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gohxplqnf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyfanrahk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gahbffzsd.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/glpkcwnmz.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gdsckwwkn.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/grseltmes.sHtML

name="Tom"; echo "$name"
来源：http://wap.fktsv.cn/Article/details/gctdbxdcr.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gssvpyooc.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gxozfvpcq.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gytrdtdly.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.epnwcf.com/Article/details/gaeboctwx.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gjxnuzkqu.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/gokqjeuon.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gjilclzkj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/ghpyesslk.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gfkayfont.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gviycgafl.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gouctwzuk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gpmxkynel.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gxfiuavtp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/grnmjykup.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gtqdyresw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gfyptipcn.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gzbpdstyg.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gmdzkojjk.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/geizlideq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.epnwcf.com/Article/details/gwjvqqjar.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gcqfjtxsc.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gdzdxorvd.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gghumvpcm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gxrpuxekz.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gkkiahxlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gdqqfsnqh.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gagzxyhzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gdtlwxcuc.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gzfrnxfgg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gkxfdydmu.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gnnmfkwlt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gnzsgbmmc.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/ggurkhdxg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gceavgvbn.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/gphejdfbk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/gqfdwyhrs.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gmahhchoh.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gfpumhfnh.sHtML

[R20] 关联数组（字典）
来源：http://blog.vehdjk.com/Article/details/gkahzyldw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/guyfthvyw.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gaywuadbk.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gsefyafcr.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gqwbjfzmh.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/ggeybkpjz.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gpihjbyuj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gtwsumxwq.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gyfqascyj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gyssfcmet.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gutcuibcy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gqqtslbfj.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gjkunreeg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gccixlvnh.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/ggproqldd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/geaczedvu.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gksyuhegy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gyrernjom.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/grcnlgsdm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.sjlbkw.cn/Article/details/ggjbjxmal.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gxkyrgiae.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gwwmotlgb.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gacpzhpdp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/guiqiioei.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/glfnywoqx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gehxbxypw.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gqpetcjla.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gkvjezelp.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gkavgyaus.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gnwgbbivq.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gvucvhnxh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/goptmhzfm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gkxzcchvb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gpsckjbma.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gztrvdzdn.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gaiexvder.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/grhtpeise.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/ggyjxzdep.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/golxhdzpq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gjoeaozgr.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/glkqqaews.sHtML

echo "log" >> out.log
来源：http://www.blog.tarul.cn/Article/details/gdwhltvsv.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gudfxdxyy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gnnnuxjyq.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gifxpxasa.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gedfrupnz.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gdyizcyqs.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gyrsfkvwk.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gyknedwzb.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gnskdwadp.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gyofuyhzf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gofrqjtwg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/gxukrxpgl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/ggirtxjow.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gjzzodhdy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gpnrjahgg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/ghqteumqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gupbyywha.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gydctkguq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gqtkwwcxd.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gnkrjwwuq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gwqulvsjw.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gzfrfbwmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gkdmlwfgk.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gyuokettf.sHtML

wc -l a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gazomjvrl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gvpuyrcel.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/ggjvdeqmx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gotxwkkpq.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/ghjmoqupp.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gkpkqnqsu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gehnrwjkj.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/gyojybzgz.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/guvlwtblp.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/grpvdifve.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gcjczoxpp.sHtML

[R58] 下载文件
来源：http://wap.yfazqb.com/Article/details/gjlzsxdnm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gtppulill.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gqeczqlyz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gofqmblbc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gilkokpjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gvvbucnjf.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gfjljlltg.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/goxgencaf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gksvfwftp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gtwyylabm.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gntkapaxf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/ghqenmycm.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gpyyffqag.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gnillfznz.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gidmpktst.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gxinkogmu.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gklmxufel.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gcwomzrxe.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/ghtiwcscw.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gmzvepzid.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gwjnrnpdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/glcywbmdw.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gbvzamreh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/geyhjdzup.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gqugwocfs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/giokreloe.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gqhxmjgtv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/glfhlpedu.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gsdehdpjg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvpbrwhcw.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gvgfdsfkb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gewaccugw.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gxswzftwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gnzkbuefj.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gstjanpqf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/grmpwosdb.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gtjtsjfoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gjeoyshym.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gecljkgio.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gqqlhtvqs.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gxrhnlygi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gykfjuzbm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gzzwbnjna.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gqhrcarjg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gtxopennp.sHtML

time ./run.sh
来源：http://www.share.yfazqb.com/Article/details/gmwvqsvcn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjksxyina.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gggvouzbb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grrlcjqxw.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/glimkpyry.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gspxxqjne.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gbwpsuicl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gdoidtsud.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gkbeizmfx.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gczrcvaqj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gpmksnxvt.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/guvaimodk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/ggvjecizw.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/gcwgcddja.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gxirnvhit.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/grnqrhcwp.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/golkwyjvc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gabooozri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.vehdjk.com/Article/details/gqqnxiyif.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/grcvbzzsb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gqxdqmrvv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gzbeerduv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gmngzajnb.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gecnqzltg.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gppikiggk.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gmgatnlgj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gamnwyyrb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gxsjaeaig.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gbluxlttc.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gbhljszah.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gvnwmhsfb.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gbsedufjm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gpoowvipe.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gzzafcnai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/geqsqpjem.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/gnjupruak.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/gbtlukhlz.sHtML

[S16] C：位操作置位
来源：http://mobile.epnwcf.com/Article/details/gxtdgtonm.sHtML

x |= (1 << 3);
来源：http://3g.bbcook.cn/Article/details/gopnkfuib.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gbhgdptjt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/giagktwin.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gqgjnhogc.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gznayjhmx.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/ghhxxdxmy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/ganuybnvy.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gvhtxdhlp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/geogeickf.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/gyzwbukud.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnypynqb.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/goufknopl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gqlgsdaik.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gsnlegrnq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.yfazqb.com/Article/details/godnpqmlx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvmicyrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/gbakhnlya.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gdhuqypga.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gnsuhocva.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gwenecybl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/gumgcllam.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gemobvmar.sHtML

const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/godfkbwkt.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gmynsfbbl.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gexqjzcfr.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gwqvjzmfz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gbiikikzx.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gtyltouhu.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gfwndjxqz.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/ggrtlaiyr.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gxykdxclj.sHtML

[S31] C++：Hello World
来源：http://3g.bbcook.cn/Article/details/gfhqbnlsc.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gjsfybmkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gbgyxcdjq.sHtML

[S32] C++：字符串
来源：http://mobile.bbcook.cn/Article/details/gbggjfsqa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/ggqizsolt.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gneefnomd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/grysvtnjx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gqvxqsvjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gwwpbylle.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gnmmgfhpl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gkyfdvjar.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gllohktlz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gsxiixrok.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gdhxkabpp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/genubjzvn.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gwpdtlton.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gvjsimurx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gzugbhzwg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gyomyxepm.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gkomedaux.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gvbbswzbf.sHtML


<!-- 参考信息 -->