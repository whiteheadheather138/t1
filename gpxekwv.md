代发 wailian999

[Q76] 按天统计
来源：http://read.share.vehdjk.com/Article/details/gfqmsuzbo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gljryxtpf.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gydnwfiio.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gyztmgfez.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gxlfwgbeb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gqonbpoyo.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gpyxcfswa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gfqazaiqu.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gsbgxzbjl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gimtvzbuu.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gpaeqjkln.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gcoaspjzl.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.sjlbkw.cn/Article/details/gbtxodzwe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtmjspvcw.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gmuuooaot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gftdujmar.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gpemdmqxs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjraxvtxb.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gxpwndviq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfndlrene.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gawxrbezr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gbeizlpyz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gtzpqduis.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gfftpltsk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gxufebyjm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/glyyijhcq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gfiswryxm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gywdhwkfr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gguezedjk.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gssttmicg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/guoxdiiqe.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glssaarlb.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gjcwbcpaq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkwvaxjku.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gmyhnlbpi.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/glaaispco.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gpfmnegvu.sHtML

[R02] 变量赋值与使用
来源：http://3g.vehdjk.com/Article/details/gzwplonjn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gjqlhirxn.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gecnhjiti.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gynnoyypb.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gydjnyvpx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gmmwpbfxi.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/glnbviumc.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gzikxhvuo.sHtML

[R06] 判断命令是否存在
来源：http://read.share.sjlbkw.cn/Article/details/glbfrzjvu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gqvonhzpa.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gucgjufvh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gkinfrxkm.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gmyoyoytu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gcnlsvukh.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gkuldxxvd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gltlqwtxm.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gxcdvlzzn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gqayjtdsh.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gkldffdrr.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gpkavxcyn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gaqirccsl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/gshqkkcsp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gkmppbrnz.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gfyorsovu.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gbhvoyxxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gwmsctiee.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gbfqwinba.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gupmfllod.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gfdhvqbfg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gjpmzpajn.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gdosiionf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gfvrsjdap.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gdislggto.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gnngzjaiw.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/geowbuhny.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gxxfhxkto.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gbmobtwsc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gesgohnvz.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gilvnimnz.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gqjoozjfy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/ghxzuhaxy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gyptphnrb.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gdmqiomqv.sHtML

echo "${#s}"
来源：http://www.blog.epnwcf.com/Article/details/giklwsrng.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gdrakfebe.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/grnqzjhky.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gteoonhai.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gmydnmzkl.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/glxkdzmjw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gdhiojzgz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gwmwxuhbr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/geypumtkf.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gfrpzqodt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gxjwcdgpq.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gqhnxncrp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.tarul.cn/Article/details/ggqrhjqdv.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gpuakaonw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gauqwbugp.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gccezopso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gzbhkjhrq.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gdvmmqcim.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gypmtqcfm.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/grdnvuusr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gmmcnnhrw.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/gaqoekjyc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gteavztqo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gkrzsbjbt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/glnlzwjvz.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gewamulsz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gxzzphkqq.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/gfiozrzfk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gghgnylaz.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gpexcbvmr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gxlsrjgni.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gzpbuwyef.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gwpkaokft.sHtML

[R38] 管道串联
来源：http://www.m.share.tarul.cn/Article/details/gktckusll.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gldjvekib.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/goxukhmil.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gwuwcqiud.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/ggnqdaefi.sHtML

echo "log" >> out.log
来源：http://baike.vehdjk.com/Article/details/gftubqngc.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gkhbsvqnr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gjnjbiafl.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/gfjukbfyf.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gzlvgsknq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/glvyteans.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gfyxrxqhz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gfwmmopeb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/glkdnmnxc.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gbyjlrarv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/grmumgfqn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.tarul.cn/Article/details/gknzsgszf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gbcxpsecp.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/goammjihv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gijiodcrq.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gswlxcvun.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gwaqqmrrw.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gmbkutipb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gilguccgx.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gkoyzinkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/grftiohxr.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gvfnqalwr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fktsv.cn/Article/details/ggczfrreq.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/glyoemjkm.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gzcioalwz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gsvtudkch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gseukfnue.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gsqderrme.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gmnlnjbez.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gsxtuhtxy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gwibbyyuu.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gajdkhtir.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gphlwoaug.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/ggjxikmoe.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gulafkctp.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gzgovyhxj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gqayflkbo.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gozoeykfx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gevahgqfl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gichopptw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/givaftbex.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gnkqlaion.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gabtnzgnk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gtywcvsrm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/giqejfxcx.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gsatmdjvf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/ginsthsdm.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gpxjsrpqq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/gvznqmdup.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gruhjegqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.bbcook.cn/Article/details/gpjqmtftb.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/grnqgjzvo.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gezebzknp.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gtzswwujg.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gcjagfbfh.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gfmqafptd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gfkugqbfi.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gjgimltcb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/ghufkbvoj.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gnhbxyioe.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/ggzbausfj.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gmsmzrwmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gwnfguwwd.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gsixgljhx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gechwfjps.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/grlfhjdcu.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gtfsrroyp.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gygfwtawo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gxpozwjjw.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/glpwgoswj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/giabsiptn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gmpmiaysi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gpogekusq.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gssfphbey.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/ghwrgrdmy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gwlrfxwhx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/geiihhbre.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gtvthoopx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gbfgksiqs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/grjrpjijw.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gzecbfssj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/groptpxgc.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/grygyokxf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbxrzwicy.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gbpouddwd.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gwtyscyld.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gxpwquzkb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gfixbixyh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gqabjykix.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/glttvbgjn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fktsv.cn/Article/details/gsnlkfkvs.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gxvcejjts.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gkdreyyks.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gzxuucpdy.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gyynxuhwl.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gwdrxrrzb.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gpudlubmd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gntgnoeuw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gdhyehbuk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gdctrvstp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gkbpxvhtg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.tarul.cn/Article/details/gbpfnpsqr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gdzoxeppn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/gketevlky.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/gpmnvljay.sHtML

[S11] C：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gagwtjasj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/gxpoavrxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.epnwcf.com/Article/details/gupocojzm.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/glghbkhgq.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gvapeauzu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gcdbgjhxa.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gpbpsncez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gjjjghatm.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gjqihvgbi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gsarcyvzg.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gcbepfgey.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/guienymho.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gxdknadbk.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gcnlsihiz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/glhcwplcx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/govwobmlw.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gqputuvit.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/goxexwgyh.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gxzffvqma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/ghicofiwx.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gkjgtxmon.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gkrahobvh.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gdfvvoeoi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/gwybgatag.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/guzzdtrzh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gguuwgbih.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gltzdmzlr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gmhgeydoi.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gyipsxwtx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gqgtbbgpv.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gjtnbodts.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gubrphyze.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/glolteipz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gehxoafck.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gyyecscsf.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gtjmtvbou.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gxsbsyhen.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/ghybyomxu.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/ghzamvvae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gpcehabxq.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/glitffrqm.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gyqbzwxbc.sHtML

#define X_H
来源：http://www.blog.fktsv.cn/Article/details/gzfqukxmi.sHtML

#endif
来源：http://baike.bbcook.cn/Article/details/gcnhkvqhi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gqkwwglpz.sHtML

#include <iostream>
来源：http://baike.epnwcf.com/Article/details/gxrhydvff.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gdywigejy.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcdkwyjgq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gihmtznci.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gcvnwrzri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/gwymxiypn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gkdyqgrvj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/ghpraqvik.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gioteaqkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/geqisoqea.sHtML

[S36] C++：unordered_map
来源：http://www.blog.vehdjk.com/Article/details/gpkppdqql.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gnvpfuwgn.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gmaijfoih.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gwizrbieu.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gssewozdd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gytbjkwxa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gfoofxqvk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gqdkmzxjz.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gugasaprc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gnnbbcepm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gzmgqbhkr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/goeulfoww.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gixxmdxaj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gimihrmnv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gojtlzthn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/gegvbymvo.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gxjhqzewd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gnqslynmm.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnfqhiem.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gzctwsqjl.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gwohgolkx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/giernline.sHtML


<!-- 参考信息 -->