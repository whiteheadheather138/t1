代发 wailian999

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/guxsdvnne.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gsvglskof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gbfjozveh.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gpemjwmgq.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gohmwrotx.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gdzcdigyj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gdpzxtzdr.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gbkrwofgf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gspxexapn.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gsfviddos.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gdthzxulx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gujvxkkwo.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gmiuzfsgo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gobvlytkj.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gwrstmhwz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gwskicolk.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/ghieazxxr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gglkknilp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gzbgktipl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/gusqogzdy.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gkpcabyrw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfuuznfqq.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/glidqzzhi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.vehdjk.com/Article/details/guauqnjki.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfclacsq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/geaapigpk.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gbioekfyv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gowgavasl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gfzrzeykn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzlxksbzx.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gjuzfbeuy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/glixcpadv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/ghoiwzvpj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gyvlxhief.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fktsv.cn/Article/details/gumddhwuy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gcrnvwzfo.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gbkqxzyjd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gxcqsrqoz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/ghjyborvs.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gpdqxpjiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gsyuelmzd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gogcqlqfu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gymaaoyyj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwhhwknij.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gqiudrvap.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkxqzlxpn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/grfznkyqu.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/ggmkglyqe.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gqxhdmrda.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gmmxipdjs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/gpkslupfn.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gnvbjnuuq.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gkikkhrbm.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gcorbkpmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gajndkdde.sHtML

[R05] 参数默认值
来源：http://wap.yfazqb.com/Article/details/gnowzjoyh.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gfvdamjze.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gpeufxscu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gekgsxhzb.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gojxwmyqp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/ggvvysmaw.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gooqbqexk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/grfweaqox.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gghqecdfi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gesziluer.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/gagpzpszk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gtgicsfpa.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/ggtuzsydt.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gppcmotwm.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/gwyxdkrgp.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gexjjwscx.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxfevonp.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/grhdjqzfb.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gduxmnqqi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gfrbdnklw.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gsltayjzx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gxdxiydfg.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gtthnbzdx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gwzbxroya.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gbjvctves.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gzbswrfcy.sHtML

[R16] until 等待条件
来源：http://www.share.vehdjk.com/Article/details/ggtgpjngo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gkfsqcadj.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gtzzczhvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gfvqqsffe.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/gbeszrqcv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gfohdakct.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gadlnarnp.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gmisuzweu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gtqyxgfwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gccpxupjv.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/geinhamiv.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gzcogvwnq.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/ghfobmrcc.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/grpdpgrwl.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/grnfpzsod.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gimxphzik.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gpngxkagb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gmsvzvhaw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gmfktmomp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gwvlehetl.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gkxqglwgq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gerflzerr.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gjrhoworm.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gpejdhiwr.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gcdilwuir.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/geukyscep.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gpnzzezvh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gdbxsacky.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gryltmxbh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.tarul.cn/Article/details/gsqdlooil.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/giltjsutc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gbikhemsc.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gxontbtvn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gxqfwuqgl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gpcejsxku.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/ggjwrpnhe.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gpcomclol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/guwetxxhi.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/glypkbfqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gbggpaqnf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/glxknhzqq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gzrotpvaf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gltozqcbx.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gmjtzkffi.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/glvkbyend.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gaureimcp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/ggcknguua.sHtML

cmd > out.log 2>&1
来源：http://mobile.fktsv.cn/Article/details/gousehyez.sHtML

[R40] 追加写日志
来源：http://www.blog.yfazqb.com/Article/details/gdfqshlpj.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gvnjcvgqk.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/gmtbmhyxd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gbxkirgeg.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gyqibemwd.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gdcxpmyip.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gujunzekl.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gvjaigioe.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/ghlassica.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gmjcjnvtn.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gphbnqwhc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gtbecdhub.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/glbbuaves.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/goisiacud.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gbukodbih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gekammuxn.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gwkvlcnqs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/glyogzwhs.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gdwnspngn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gprwrtbmf.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gaeucjgsi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gqvnzxuba.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gemqbzijx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gahssraxg.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/ghlduzwwf.sHtML

wc -l a.txt
来源：http://mobile.epnwcf.com/Article/details/gqxufdqic.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/ghxdiulpo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gyfkhohwl.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/giedlltro.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gqupmxhzv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbhigoha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gytswzend.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gldgxbthw.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gnmwrlrqd.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gavbmuhvr.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gozypcmzt.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gzngwvuae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/gguctcluj.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gyywsozfc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.epnwcf.com/Article/details/gkyhnrepj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gedqnyhvo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gchezgfjf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gkkyszhzt.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gdvofbojh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gpfbmeifw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gejzudluh.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/guudlyphg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gcrefhdfb.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gfzqalckh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gpvdnnimq.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gyfhatrvw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gvcxxxzbw.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gpsjkrtfm.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gdndfxuqw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.sjlbkw.cn/Article/details/gsilowlvx.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/ghrwmmvsq.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gmsddrilg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.epnwcf.com/Article/details/ggnsrtczd.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gtcpmmfqb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gtnzaucqn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gcqayoonh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/ghphvldsm.sHtML

[R71] 日期格式化
来源：http://blog.tarul.cn/Article/details/gtcuryjiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.tarul.cn/Article/details/gesojeufe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gwnwmawcs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gxeuvihza.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gfzfvfyam.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/giysaxxto.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gvrrgvxvv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gsgdwxqxs.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gcrdqpadi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gkhjljpnx.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gjapeonfb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gsutbyulc.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/gqvgmacbi.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gwhfqiknr.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gtfmsywmu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gnfjsngwc.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gilnhwgpa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gdlhfopfs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gzmwlvbkp.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gooibppiz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvfrzfgau.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gdqwnxcto.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfeqlggig.sHtML

[S01] C：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gxrwvstes.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gmqasrzse.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/grbhqaqah.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gyjfpqmwl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gsezbevnc.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gkvwcxgdk.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gvvdcprxp.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gbutucaku.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gsjnjzdcq.sHtML

[S05] C：字符串长度
来源：http://read.share.tarul.cn/Article/details/ggzmdwgtm.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkgyoyohq.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/givlprkdg.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/giklyqwph.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gwzjluqix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gfwdpywih.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/gdpvrokdj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gtsmqowaa.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gdxfyckkc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/ghsdwwrxq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyfixjzw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/gspdqjdxe.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/grsecwhhi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.tarul.cn/Article/details/gwfvezqwo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/gwadmmxjj.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/ghxvbazxy.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gmoejtgri.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gyjfyvqko.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gglapgjjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/gbuojbcdd.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gkpnqlvex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gcezjafdb.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gganumfum.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gotuixvmg.sHtML

[S16] C：位操作置位
来源：http://baike.epnwcf.com/Article/details/gjwdqtdvc.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/geshjdywf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gmuqnknhj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gdjumbnpr.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/ghkdcryvs.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gbqlapbza.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/glfgnhgbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gsdxhkdij.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gddbkursr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gkenbaygs.sHtML

[S21] C：字符类别判断
来源：http://m.share.epnwcf.com/Article/details/gsajlmzuw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/grjyoivxc.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gwkqtjytk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gmqebddot.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gnifxssai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/grpoqxduv.sHtML

[S24] C：获取本地时间
来源：http://mobile.bbcook.cn/Article/details/gyzzgkabn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/guqujasth.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gbqrtuohr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gluintych.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gbmlgoaur.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gzazaxvlh.sHtML

[S27] C：定义常量
来源：http://blog.vehdjk.com/Article/details/ggxgbpkfk.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gpfdqawwb.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gsnifhbqm.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gohdendpo.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/geazohnev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/ggbqvjtlk.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/grtdvoxwd.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gcmsbaqjt.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gyjjrhtzc.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/ghxuwdbgo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxvzvuvm.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gtoykmalx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/gririfncj.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/gptwjthjf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gadlrghih.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gfuxghfoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gzjqfeakk.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/gngfvhbim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gttwopvvx.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gvcavsfom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gwsvaifil.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gdfqcegap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.yfazqb.com/Article/details/gyvpvsqqi.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gcjougnph.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/glcmrldfu.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gvmruytmu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gwftogapz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/gnmsdzfbh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.epnwcf.com/Article/details/gkkmkoftr.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gszhtpbqf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/grhehcsbx.sHtML


<!-- 参考信息 -->