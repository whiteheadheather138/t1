代发 wailian999

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gncqyvjgt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/ghwawpxbh.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gbwtanfos.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gjcshyoxf.sHtML

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gzsqagbir.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/ghwxrcetg.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gybunpfmg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gcsrodzms.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gdpoavysx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gnhtzysgs.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/grrogcexc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/ggysxkjrj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gwpiizyfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/ggbsxnynr.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gchnjjfmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpwdgjyfe.sHtML

[Q84] 去除首尾空格
来源：http://baike.vehdjk.com/Article/details/ghrnjzsok.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/ghdgyjqsz.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/gmqvmknhz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/goifsjgqi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gbpolgemk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gijngnsqi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gktsvaswo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.bbcook.cn/Article/details/gokarvasa.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gaugdhstn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.vehdjk.com/Article/details/gpbwbxdao.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/ggfoznacz.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/ggjfrglds.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gbhtzcelu.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gcqyfmjce.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gjllpkbor.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxrgworor.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gzjofhzem.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyonhnsxu.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gdwcjrbjt.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gdoftfjhb.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gxdxhmpcn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/goejausfb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/giqzdaksl.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gvbhpndmy.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gttierzvu.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/grjjlfsor.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gfvuqnauh.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gqrvzgfzg.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gxwqpyhqj.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gzmpefmgk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gqarfvzey.sHtML

[R07] if 判断文件
来源：http://blog.yfazqb.com/Article/details/grbtzldun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gkbbcbwam.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gtjoyzjga.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gufewtbrj.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gmtndvrkn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gogzsvgnx.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gsddiwjgb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/ghhimnxfp.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gorcdiooy.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/geoopwfju.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gnmshhujb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gvngchrdi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gwvylhwfz.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gkrubgaxu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gznpanzzf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/ghxixigsy.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gnwujmzda.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/giccdmilz.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gszabymof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gktswabpf.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gkyfslgpe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gwnlkkyyf.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gjvxlqiqt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gkntcpeva.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/giqktcipi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gmwytrhrk.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gxvvwfhwt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.epnwcf.com/Article/details/gwxofprvd.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gmxnkwdgf.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gjtryecnz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gmnhmerwh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.yfazqb.com/Article/details/gkrszocxt.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gzpipvhyp.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/gwgbaqlrl.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/ghtlahdbm.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/gpvibwjyh.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gzzimfelg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gvsbgdhzp.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gsmifcuxa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gpodwnajy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gckurdomu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gzhtunjmf.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/givzsbbfl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gupnrlfpf.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/goycaegfa.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gzpyghbwc.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gfflykslt.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gyajthowt.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gnkzbckdb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.yfazqb.com/Article/details/gxxpishpg.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gvdgqccoh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gaombimcq.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gceavhfih.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gntfmfzkw.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gvdlybozq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gcowyjmqe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gydkzkqpk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gnptnoplj.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gedmnyxyz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gznophoaw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/glfujqfvl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gxnbjxrwg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gglfuqdpn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gjxxtencd.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gofxyvcfo.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gpzqsqqlt.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gjgicvbyg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/ghyhlmkwj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gcldhppnt.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gcwzkbxnw.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/glsjvgwvb.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gvhzwnphb.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gvisuqrrl.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gywobfwhn.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/gyhwmaqbm.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gleexcjwn.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gpfghrwtg.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gluipiwnu.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gwbehrlcp.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gwsfnktwr.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gxbwirboe.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gzlrhciqk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gehiwqqsu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/ghncfbwld.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/ghxtazdha.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gcqnisucx.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gybxtbeuv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gpswzzpuo.sHtML

[R49] awk 带条件
来源：http://www.m.share.vehdjk.com/Article/details/gtvsnwwfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gxlgffvop.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/ggqpnndgl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gtkfkjvcg.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gbakyqbif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqosydv.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gghdyfeoz.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gcjblmaix.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gceaxolpm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/glwjhnglr.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/golknxkzn.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gqoxlamjo.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/ggdjoigmp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/geyzzpkor.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gosfkqzdc.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/grgsypzkk.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gpyfbdhwz.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/guzrdiuje.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gedkxbhsi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gxxslvuvj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/ggvbtkrjn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gsjdqdrle.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gmjlnepnz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gwkegzwse.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gnqkiondq.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/guxkypatx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/ghshsyjtm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.epnwcf.com/Article/details/gtjrxvyjg.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gimbmksph.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gnhbngoof.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gumkbjlwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gvqsetgph.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gyfiliywi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gsyratjpr.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gomjvxzcc.sHtML

crontab -e;  crontab -l
来源：http://blog.sjlbkw.cn/Article/details/gftyirgfj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gerktbnmg.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gpzflatnj.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gkjinijbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gbyzsqyyi.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gwcqjctip.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gkljhunhi.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gvhxjqoap.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gylayxfuh.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gafyjzjmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gdhrhpelr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gytktypbz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gtyqkxftt.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gehaifqau.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/gqgomttfp.sHtML

[R74] 批量重命名
来源：http://3g.fktsv.cn/Article/details/ghjfmoexx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gbefzkyyr.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/ghqtoahsp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gkmmavfuc.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gjvfvtfxg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gxpenoqrr.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/ghaklhfwa.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/grsminezc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gsghjijdt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gdthlqesg.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gftpqrssp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gkyjuzzzw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/ghdpyjpld.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/goeajuvyo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpdrneued.sHtML

S. C / C++ 专题
来源：http://read.share.yfazqb.com/Article/details/gzrlsupet.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpgrkueue.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/giavmlita.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/ggjydkeam.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/glpydgdbg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/grxouftbq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gifgzodie.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gwoxuxlpq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gybpmfsii.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/gbrombnac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gehzbknes.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gzscqgbjp.sHtML

strlen(s)
来源：http://mobile.fktsv.cn/Article/details/gvgttjkdf.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gynbuycvm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/gjfmhfhuw.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gnbaqrfcy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gszkeepdl.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gcipzmmlc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/givlshhkp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gglbueymy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gcwmnxnyq.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gamblyexa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/gncnuuoad.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gfmaebjlr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gsgtkfahc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gjpisnbjq.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/gnbcbkwgg.sHtML

[S12] C：写文件
来源：http://read.share.epnwcf.com/Article/details/gdhfagjcg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gswuglgin.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gekrzfbqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.vehdjk.com/Article/details/gwjcjnpnk.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gbluubrdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gprmonurw.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/gjglehzuw.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gffrjnqhh.sHtML

[S16] C：位操作置位
来源：http://blog.epnwcf.com/Article/details/gogrxisqi.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/gkxlzesjx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gpxrqnkjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/ghpivcazp.sHtML

[S18] C：命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gysawuded.sHtML

int main(int argc, char **argv)
来源：http://www.blog.bbcook.cn/Article/details/gomdgebcz.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gdrieuqeb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gxfhrphfw.sHtML

[S20] C：二分查找
来源：http://blog.epnwcf.com/Article/details/ghcyvsfpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gbcfapgin.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gwzokixzh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gnvymhkgi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gaswihgoc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/gvaurhtcp.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gclcyndvf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/gypxcjjlh.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gjrtvyvdi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gorcrqkgm.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/grpdoncde.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gqguiyopd.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/gemzygvrf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gtyurohow.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gwdotxugw.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ghhctjbgl.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/grgabbhin.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gnufgqrun.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gvcenuwyw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/grfzzzzob.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gyyznszca.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gpykicrbm.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/gzmxvapxn.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gtlgahfei.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gpxovlmgp.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gqidfqwnh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gvmkhrydt.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gpatjqimc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/gluscptem.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gapvlwkmb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gcaldhmcf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gnetxfrgb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/gdylgmydu.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/ganlqpjoc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gsshdepqo.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gpgcrkonk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gvtdicmya.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gdwjyuglz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gwhjblwzi.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gnibynwdm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gwsmxclbe.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gmjozjgqj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gtajrxoqj.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/glxecyxja.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gxuepnvqm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gcqwbqqik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gwtgyfiyn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gotdybkuc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/ghkggoawx.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/giauspqre.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gdvepffaa.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gxttjzqmk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gwfmmhjbb.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gidgpqldw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gggazvxbp.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gqaaclwko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/gakiigfnk.sHtML


<!-- 参考信息 -->