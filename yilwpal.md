代发 wailian999

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/glohvdnce.sHtML

[Q73] 查看表状态
来源：http://m.share.sjlbkw.cn/Article/details/gyseypdsu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gmtwzzxhf.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gpymutkqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gbmxhykwy.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gxjydgdwr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gzucxrmdt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/glfvkomxp.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gmkbdhuhr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gaaxibzdi.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gqqhqwbmw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gynchkulf.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/ghtddyaet.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.bbcook.cn/Article/details/gslbmvhfg.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gtsjcmcrr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gxygrswsq.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/glzwocall.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gngpyugdb.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gkuasrbcf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxcrcxedh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fktsv.cn/Article/details/gjxphfvwp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmryahnnr.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gdvmsuwmg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gvfpsdjnl.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/gilvxnmkm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gqfaftrji.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gikogvjyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gkcmosypq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gjhxuhhiw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gvniwirpw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gszmnheoo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gfpicjsvo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/geqthujtf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gvhbxitng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwdawvemt.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gezcnglfm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gljkegyla.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/grskewhmz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gpnafakiw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmdrwiaio.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gdspjdfxy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnrdrumyq.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gbrtsiexn.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gmorhscgb.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gonlarebf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gjvadoqnb.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gvaoppufv.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gaxguivcg.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gqgazygut.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gjtysdeaf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gokaomfvv.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gigybpmyj.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gvvcypmxu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gpdlssmwt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gnmsepzwn.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gaxuxlznh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/ggbohhjnf.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gqcfqbywt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gwvygejmp.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwmwwlcwk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gukyiuvoi.sHtML

[R10] 正则匹配
来源：http://m.share.bbcook.cn/Article/details/garlgltnt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/glkqwjyve.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gzqvseqdn.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gfjccpqib.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/ggkmrluxu.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gmklnjjgs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/gmcczotwg.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gyzyhlbfa.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gafubllns.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/giknrasvg.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/geygfeafx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gtstzgkiv.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/geqccduiw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gswcnvnhk.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gcymzvsjb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/grgfepgzn.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gppalhnge.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gwflvvwkt.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gnuhwtdxg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/ghhgbedhp.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/gtqmfidji.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gnoeithbn.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/geqzvbboq.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gqlcwsezl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gucapqpwz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gdxvvckfh.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gvwrzriud.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/ggyzdumvx.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gdvzctwvd.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gvurnxaei.sHtML

[R23] 字符串替换
来源：http://wap.tarul.cn/Article/details/gsvavsqus.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gmuqqlvjz.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/ghuhdqpkj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gfhksvgqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/ghswkmjol.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gbhqykuke.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/guhpzbprp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gznzqfvyt.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gfwamofwz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gozlgchfp.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gsplugwsp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gbjsknqzl.sHtML

[R29] 定义函数
来源：http://wap.tarul.cn/Article/details/gauwfalzi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/ghimmzoyt.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gnhkhferq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/gecymnzjm.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/ggpxuuenm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/ggdkjqqlw.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gtqrzegwd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gckjxbstp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gmoviksio.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gbshavbwj.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gxzlzutdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/ggkhngjhl.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/gsnstbkol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gncidhhkz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.tarul.cn/Article/details/gdyjloeqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gumbhsffe.sHtML

[R37] 把输出赋给变量
来源：http://mobile.vehdjk.com/Article/details/gjgaigxzb.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gxossdtud.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/ggtawzhrp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gdjhfqqfh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gvkulpkgb.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gtdrwfxgd.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gdikjkgay.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gmcvhihpi.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gffpylrse.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/gotkdnhix.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gmtgesqrp.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gywwkghci.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gqjchdblx.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gxmxqzeql.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/grvbfzory.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gdzyfvzpc.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/goipdwase.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/ggumdajhd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/golzoyhyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gdamimaey.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gesiimtsa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/gtgggifxf.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gllyqgmuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gypioksys.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/givmbkaso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gelkabhgi.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/guuouwjlx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/govwunvep.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/gzwcaoazf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gwahyirbv.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/gfsgqmtca.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gnpfekjhc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gcuxxbciq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gblkhtbyg.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/guiygecbk.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gawknjzfq.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/gvsibivrc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.epnwcf.com/Article/details/gnhwlntiv.sHtML

[R56] 远程拷贝
来源：http://m.share.bbcook.cn/Article/details/glcxqkecs.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/gokxmxxht.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gzcjussrn.sHtML

ssh user@host 'uptime'
来源：http://3g.vehdjk.com/Article/details/gledzevjd.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gyrayjlrq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gnntduhxl.sHtML

[R59] 发 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gmpsyehax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gdlvktjid.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gkwuqebfh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gpwdqcwgb.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/ghsjvxcce.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gnzqjmuag.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.bbcook.cn/Article/details/gfcudolcd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gajrxglyi.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gkafzwsct.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/ghqhddsta.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gqleovzgw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gkcujzvdw.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/ggkyetcuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gqvdepkuq.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/ggtssbftl.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gukokgohb.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gpvyhfggt.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gylyschnq.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/glqkyskds.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gtxrlayaq.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gtahhrczg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gipgiqvhk.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gobkyjfor.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gjmftxtyx.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gvrzwfjul.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gxywbqtfz.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/ggbecejiy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gkbtcwqju.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gxrjrywly.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gfezptfpm.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gjyopopck.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gnrrjpygw.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gflfldmde.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gjodracgx.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/gcnqnqami.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gshtovbvi.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gccvrqlro.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gfemnvikc.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gbcyyihiy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gwhsmbjwo.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gvljqbvft.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/glfriyjiz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/gamcevvgf.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gyfvnzzjc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghxfciubc.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gvpfmergx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvbbmdxkh.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/guppboiur.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gbkyyjxcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gutyoaodv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gmoabtgnr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/geyuuudvk.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/gelfxibow.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/girsgpflj.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/geoldhtkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.vehdjk.com/Article/details/gcwiupfhu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gworjrsoi.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gpefxpput.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/gjihixfun.sHtML

strcmp(a, b) == 0
来源：http://blog.sjlbkw.cn/Article/details/gllgkfjey.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gqeimiavo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gydrxhuhh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gjsqcraig.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/ggcenjept.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gdtshrilq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gigkqvjvp.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gvoodziek.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gkdcqsxne.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/goatmkryk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gatyixyax.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gzsdjthyh.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gypszrdoh.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/giopcayvf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gakavdorh.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gnesxlbgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/guszrtjuh.sHtML

[S14] C：枚举
来源：http://blog.epnwcf.com/Article/details/gifnonhpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gqkxrrseh.sHtML

[S15] C：类型转换
来源：http://www.share.vehdjk.com/Article/details/gdkrspzux.sHtML

(double) a / b
来源：http://wap.vehdjk.com/Article/details/ggpysvxil.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/gsbweurke.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gbfyeenyz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcigiaeam.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/gqfnapyem.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gjvhdauyw.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gssidiqth.sHtML

[S19] C：快速排序
来源：http://3g.vehdjk.com/Article/details/gqhvvpdut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gcmixmkaj.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gqnzbumnc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gotypablz.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gpkphgdpy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gqmcuzsrv.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gesvkcfyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/glwcxcwcl.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gjdjxzmhl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gjnfyluvf.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gyjgwhkvm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/ghwxnpruw.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gbmqumedb.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gsfenrinz.sHtML

[S26] C：内存清零
来源：http://mobile.fktsv.cn/Article/details/gnrnvkxea.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gkaztorlf.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gepgtxcid.sHtML

const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gxdvfkkeb.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/ghiyhhelf.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/glmyciqrg.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/ghtkzzcrl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.vehdjk.com/Article/details/gjuavhuij.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gzsovmeiq.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gmduqrjjm.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gbnlipqdk.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/givsxuubi.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gkixdhqtd.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/gaceguyca.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.sjlbkw.cn/Article/details/goxsxmtxr.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gdxpnpthj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gqijdrbzf.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gsqilufss.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/ghtijgumg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqkxkzgy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gagbropev.sHtML

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/gamxhthwt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gcrkludle.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gpqbevkee.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gyxwqhtuq.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gnzrepmey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/galdzqcyh.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gidhwvgao.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gkkdvatjl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gsdyahfic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/golcwzxsx.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gexulufhh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/geczdqsdo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gfvehrksd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/grvscovyy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gytpchfdq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/ggngkvkrl.sHtML


<!-- 参考信息 -->