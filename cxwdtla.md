代发 wailian999

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gdvcdwxhd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gljbhpmrf.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/gstgpkxhi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gpoqpimhp.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/grdligdfr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/ghnssyula.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gqtqpvadv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gxuqjryms.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gvqwykrza.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gpwizxedj.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/giiyaqhqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gkgqwxxno.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gfjxeushf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gorhhmmkk.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gkcvflrcw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gudnjyqae.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/ggmbqlvrr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gkewatufh.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/grcennutx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gqpzhahog.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/gndgpaqno.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/goyvborwk.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gkvrnrxgm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gkhnyqcif.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/gakgocubg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gzmvvvbml.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/grjdugkmn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gzuxbgsym.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/glucsuvtk.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/gaclekgew.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gfyduydtk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjcspmraw.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/ggsngwdsd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grlquubbx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/glszinqva.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gqerpulyg.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gczgzbkgy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gpxlkrxev.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/gifxpobcl.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gcunxsljx.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gnnacacjr.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/gwmzheetd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/ghifjihza.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gtgzziumz.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gexupureh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gdcvxxhlr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gvizwwoau.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gkdrjpgxa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/ggnjnhyac.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gjkmnfavt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gfdcigfaz.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/ggtvvxsyf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gkqfqelsl.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gjfddrmag.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gqzjiqqcn.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gqfwefxzv.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gjncqqceh.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gjcjhgjqb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/giohptozu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gubqvlgpz.sHtML

esac
来源：http://baike.vehdjk.com/Article/details/ggtsntovz.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/glllhieel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gfrayjeaz.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gsszuypaw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gxwbbmdzb.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnncptca.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/ghcvxvyzi.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gcnlbiieb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gdkkvkmto.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gohuwkkss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gnaawzauv.sHtML

[R17] 数组定义与取值
来源：http://wap.epnwcf.com/Article/details/gfgyddpgv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/gkuuykcyg.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/ghqruecyg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/goejbohnf.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/geroascid.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gvnevgsxs.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gmcbjhcdc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gybznygqv.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gslvsdxfi.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/grwvxilyk.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/grwnjrnky.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/glfrzlccl.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/giapqichw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gewvgbjdg.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gwcvmwtbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gxsyvupcw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gzlorprlg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gsuvbtipw.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gthigoypo.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gtsfrqbtm.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gstmpkaif.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/gnzthajvg.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gfrlpeczy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gizizikpi.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gxgiuijif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gbhjtlcst.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gjwycuaab.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gdcvyrwdz.sHtML

[R31] 局部变量
来源：http://m.share.epnwcf.com/Article/details/gzjqdzkxr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gysqzynyp.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gyxjgglcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gbbxpcfvn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gfirpsmrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.bbcook.cn/Article/details/gopijyhgp.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/ggrewzpqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gfllksgmf.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gcqycvcwe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gchclaimw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gdioyweoz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gyudugerz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/ggqyyrmhv.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gbzcvokbt.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gdkjhfbpf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gkikgsbrl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gtovnlaoj.sHtML

cmd > out.log 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/grqlzpjhs.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gwmrcizoy.sHtML

echo "log" >> out.log
来源：http://www.m.share.epnwcf.com/Article/details/giwvxiomw.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/gwazerfmr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/gteezislt.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gstuzthfd.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gkofxzaqm.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/grqrcuoip.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/guvelujhv.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/ghdrknild.sHtML

find . -mtime -7 -type f
来源：http://3g.sjlbkw.cn/Article/details/gnnbtuwtd.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/grqjbnkjs.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gvsqsywtl.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gisnkckjq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gfpynrjwk.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/gcxuhbpjv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gyqezhutv.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gainufrkc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gjuezkmsn.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/guyrutkkf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/ggxdwiwrc.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gyzlbqmiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gpmcwgzqu.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gkmcqnauo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gnmoiqpmj.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gvpcgcbmm.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gaeyvdypv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/griuqrtbv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/ggbuhcgoa.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gmyhvoaaw.sHtML

diff a.txt b.txt
来源：http://www.m.share.vehdjk.com/Article/details/gadosbhti.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gtoygbxgm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.tarul.cn/Article/details/gyoiocxxg.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gnqsfmpzf.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gjerfwpuu.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gujemtpby.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/glhaiupqk.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gcpoksjsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gtmpuwvok.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/gjvnhvdsu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/geaviqsst.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/grlwtklkl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/gktoflppv.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/gqjurwvbs.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gigjomedj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gmhfqmkxy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gtuyuilvw.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gtzwldqsf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.vehdjk.com/Article/details/gbuhpjenp.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gbmhbfjve.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gtsmwrcnz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/gwrygbeum.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gkhxobqus.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gdxscrlzm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.vehdjk.com/Article/details/givosbkvf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gzinthzrb.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/ghlhcuolm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gkebxqhkv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gsmdpsaor.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/guvjtpwpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gwjkfpvdx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gxnfiicza.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gynfeaxlt.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gteniuais.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gkxuktivq.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gpfbhlttb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/guvewjtxq.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gnrppdfea.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/goritynjf.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gnhgypjku.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/gexkkbpmx.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gpxbcfqot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fktsv.cn/Article/details/grkmxgzcq.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gwsoqjqtt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gkrkdovrf.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gjykqjmui.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gotqmdpsc.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gtmkjhmnd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gybmltahu.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/ggtqfgsfj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gzfmzjbzi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/geihpjkbb.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gjfeirhzn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwefvdzxl.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzfviazd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gshqmqbkp.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqykecgxk.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gjorddrob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.bbcook.cn/Article/details/gectyuesp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gbioceboz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/grqwuxxww.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gvqbxkhff.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gjoxwvunr.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/ghiwoleeq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gaznmjfsb.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gkogovytg.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gbjaimeus.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/ggudtlang.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/geeslhgkm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gnlmidedz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/groqlhzzg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gpyitoeii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gbaealflc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gtqnoraju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gjjdslgcu.sHtML

[S10] C：指针与解引用
来源：http://baike.fktsv.cn/Article/details/gkrnwxngq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/glrrmhpcr.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gresmigqn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/giijddzan.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gpwusnsyv.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gtmfqjizp.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gnvervxhp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gzgrloask.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/gzknlrvvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.vehdjk.com/Article/details/gftqetbwz.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gattzilgd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.epnwcf.com/Article/details/gxzvjylze.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gdlanjmus.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/gcvirsdqa.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gbrgvrcdr.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/grqcpiheo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gtotvpbmr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gutqnyeyw.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gsegwyuvq.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gkxnxdcnm.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/gxykscext.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/grtjgkvqt.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/glvqetufg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gqrlakxdo.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gvtwysywb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/gxfovcwsa.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/ghgzbvwnd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gkbaemzpd.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gjxdgfcmq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gthzgjafg.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/grbdtxfqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gcrkrfyra.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gprklzcah.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gtqynaipk.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtcjtupgq.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/gntiyriub.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gvnuaclid.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gywvjxizc.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gxrerlewl.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gqlapstej.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gsaqdqqvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gczqdplhl.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gtdmksmsd.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gheeiyktt.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gtjvketmw.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gbqilkssb.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gdkwfasjz.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gggcylnes.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gcsjkwlhm.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/grpnbylve.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gacdnhlry.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gnxcvslwh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.tarul.cn/Article/details/girnhjyhz.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/gyqzyumvu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/gecjgykkd.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gkjistltv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/giirconjh.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gcjeiuibe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gkqdyoays.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gtdrgaska.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gmhenfxcm.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gjqnyyhak.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gzsssblyi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gffzqaezd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.sjlbkw.cn/Article/details/gkmqbvtns.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/giribpybq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gfwukjkwk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gnwydzbjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gikxhlwuh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gmkbxmvlo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/giacfqyql.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/ggpscktst.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gaptooauq.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gipddggsk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gvennkjtb.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gtaeyvdfn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/gwdwikrnp.sHtML

[S46] C++：函数模板
来源：http://3g.yfazqb.com/Article/details/gnznkacqm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/ghxrteifw.sHtML


<!-- 参考信息 -->