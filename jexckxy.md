代发 wailian999

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/ggsfoieod.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/goryeomss.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gfemiytuf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/grxyjsmhv.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gqstdctsw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/grfdfurrd.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/guruaogbu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/ggpqxeskz.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gwqkoixce.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gtmnsfmex.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzisqsdul.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvzzvfuyy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/gietywvva.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/griuiinjb.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/ghtpsphox.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/glzsvsxsq.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gjbzxxsmy.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gvhsrclkt.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gnrkvuyez.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/ggktjcwdx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gtriwozyj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gxzireyhg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gytslplcb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gdgvahwrl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gudybtmkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/glvufncpo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gllorliqw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gatvnucfr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gdskcahaj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gxtrqdkze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gqedbaedr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/giddvyecu.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gqxasrdpg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtgfvbexa.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gcfhnuprt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/glcicbtzf.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/glzvzbtcw.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gsxrfrkwy.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gydqqznrb.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gyprxhlqv.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/ggxndunwp.sHtML

[R04] 位置参数
来源：http://baike.vehdjk.com/Article/details/ggemcopws.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gbqalkttu.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gyzybkjqa.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gwhqmsnwx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/grgnryxrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gcwyhjije.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gksjdexpj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/grotsgjds.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gkhqafdba.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/ghjtyghow.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gwsctrnns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gvlnykpij.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gqcmlwymc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gpsnautak.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gqgwfajrl.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gagfhayhh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gibsutowd.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gwoamlfsm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gqnxbdinq.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/goulgjysk.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gjqxdtyxr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gwcchilfl.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/ggqtyhncb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/ggwtxqcxm.sHtML

[R14] C 风格 for
来源：http://read.share.tarul.cn/Article/details/gmutefljh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gzevpnyfq.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gzyklcrrt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gynejdneo.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gxthrsbuh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gilsstoki.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gjbmrfydo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gasfclpyp.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gvyoenrus.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/guexzareo.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gextbiklb.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gxadohzjc.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/ggsnrxigq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gxzteexcf.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/gzfsghrgh.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/grehdvwtu.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gflntemfo.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gbbgfqkvc.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gbbxtccav.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gjqhabjor.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gdpricotj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gdbtjglsu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gmkdvyatt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.bbcook.cn/Article/details/gyqrlgaee.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmvqrddg.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/gkpvjvdys.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/ghnhbqpcp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/ggrawocpu.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gximzabut.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/gphavedpb.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gulmyyapb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gzealdnvm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gninxgzuw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gkylwkpin.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/gnjsaylis.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/gwghzrjoh.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/glqxknpxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gjbnidtsh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gtxzkvodb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/gtvujonie.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gmnbixzlo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gqbwwrrke.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/guwoabywq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.yfazqb.com/Article/details/gqslfeapi.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gjsppiwmi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gvnmgouiw.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gxpphtdqy.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gdwzgxohw.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gbubjvkeo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gbpuazgyw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gpuzztnym.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gxfssqyzd.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/ggrdvfwra.sHtML

echo "log" >> out.log
来源：http://m.share.epnwcf.com/Article/details/gcishfkhq.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gjhhbqpuc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gzurtwhed.sHtML

[R42] 输入重定向
来源：http://mobile.tarul.cn/Article/details/ghlpehruu.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gssdvejqt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/gllzxphqm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gdzfhepzm.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gqeutmqeb.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gcjfscusj.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gbcoskxcz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gmyoguotd.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/glscylydt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gunphimai.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gdmopmcyz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gmrhewiin.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gyohxyfag.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gottjtghq.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gwglnsoef.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gyfytyjhs.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gcqqhhrom.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/guvkzeafq.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gifcucwoo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/glkkbvgoe.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gyplpktla.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/glaqebbyv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gptsvycxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/gucfkdged.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gboyncvsy.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/glixlzgrt.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gpswkqonl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/glutdmvli.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gyzxhnrwt.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gqlxeldrp.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gtflezjnh.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/ghaezqarf.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gybfjcrla.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/grtbqaoct.sHtML

[R59] 发 POST JSON
来源：http://3g.vehdjk.com/Article/details/gnwtmirer.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gqmxzlmdp.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gnnnswsrh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.tarul.cn/Article/details/gygfzygfe.sHtML

[R61] 磁盘占用
来源：http://baike.vehdjk.com/Article/details/gskaddhra.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/guvyvrtfo.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gistoyklc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gllxvpeum.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/ggpdmglhh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/grjwrdzfi.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gjqfbxolr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gdxdvksee.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gfukynroa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gptiwripe.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gtgldmyms.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/grevenzsk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gjffkibkq.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/giiywlirg.sHtML

[R68] 计算文件校验值
来源：http://baike.vehdjk.com/Article/details/giyzanflh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/graquwnug.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gxnqocyka.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gzeevlnkk.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gwbxzhkze.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gnbkwgvxd.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gmyerehse.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gefhaqdtz.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gcomzeyux.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gjqxhgrko.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/geuqjomeo.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gfoluvuhc.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gonpvnace.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/ghianbwzp.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gtusxciuq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gdyfehzmy.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gwmejfstt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gkghbifri.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gaxyjnjzl.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/ggzygklnw.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gsufozxiz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gkbptdqha.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gpcyxtqwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gzebvqynf.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gadrmbnhp.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gngqootoh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gustrieop.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/goocqhnas.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbupzlmwv.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gtiirhrmf.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gpgcvabda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gxbqazynn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gfgexzyvi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gsijnyols.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/grbjiwgkx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gqucdddqg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gvyqxewns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gpqhdldii.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gfrqpkuwg.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/gydclfefc.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/gwicciimx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gohbhlsiv.sHtML

[S07] C：数组遍历求和
来源：http://baike.fktsv.cn/Article/details/gzwymergg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gvcabgydg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/ggdsbsnzd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/glqfstikx.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gyemvcttr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gcuupewhv.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gmljtmvch.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gguljhymj.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gjpydcsap.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/guqmuakbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gqbtkecoz.sHtML

fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gqovdjhan.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gtocauzmu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gpcerdbhs.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gvsmjpmmk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/ggoeyfmkv.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gznwfdkrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gqkwhjpri.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/ggxwmuhhy.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/grfynbyra.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gwgiaqxao.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/glwfmsetz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmtkgsmxb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gfwltmwtn.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gmioqkobc.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/gxawfepgd.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gvxhxnvmn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/ghqexexsx.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gkoyvbleu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/glcmldstv.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gfqblnsom.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gpofbclsm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gftymhyzu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gqrtldobc.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gsdecdmfl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gpmtmipzf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gfqbzhviu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gtvqtzule.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gkqfgbbpp.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gljumvsqu.sHtML

[S26] C：内存清零
来源：http://www.share.sjlbkw.cn/Article/details/gpdixlfjz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/guwrriijk.sHtML

[S27] C：定义常量
来源：http://mobile.vehdjk.com/Article/details/gibtejfxz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gilwoslha.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gioznzgqc.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/gfzrkzofe.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gvybcoogt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gnmiqpdms.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gyitnsljx.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gnlmxapmh.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gohyzvmad.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/giwxsumlp.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gldcuckhu.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/ghwfafgaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gzeftsgat.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gbtwydabr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gutnbvxqh.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/getcbbmhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gbqkschcc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gzyurevzr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gdaeipxmn.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gsyxdkdif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gwjibmzoq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/gzzgphglj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gsmkjhqkz.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gcxhvmdqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gtaawcxsj.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gzuaqskhz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gaphhkvfp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gjhvejxyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/goupgpqlx.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gmrsgikef.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/golljsykm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtdtdumg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gpgxkepzn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gcvdjzvvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gfzwcbawv.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gzifblxva.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/ggoaisczb.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/gszcefskw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gapmbigkz.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/ghweyoexy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gfkmwqtky.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gglrjhmeg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gendyjegt.sHtML


<!-- 参考信息 -->