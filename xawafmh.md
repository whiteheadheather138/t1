代发 wailian999

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/garkgowpv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gickbzyuz.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gklhatpex.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gyasdapzq.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.epnwcf.com/Article/details/growlomes.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gqsnevcdi.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gxcevqaps.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gjijbskqk.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gnjlmwhns.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gftuxxqzo.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gdbqkhmaz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/glhlxrgtx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.yfazqb.com/Article/details/gqatqfueb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/guaizxipl.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fktsv.cn/Article/details/gecblpudd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gxebbnhks.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gqzosuene.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gcexwfywp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxnklqkgo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/ginkqtepx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/gpugfgsyr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gzeeojexp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gauibwvxu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/girrmsyqu.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/gcudtttha.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxjklgdxh.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/grlkfqdne.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gcnqojrhm.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gpowmivvn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gtlscriji.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gnmngjwif.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/goaashfdg.sHtML

readonly PI=3.14
来源：http://read.share.sjlbkw.cn/Article/details/gfovanwhg.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gmygeuxfd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gfbvvejih.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gkaskontd.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gyxhbdrrx.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gknsttbkf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gvfkqqcze.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gnndhosoz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/gueokocpe.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/gwidwkocu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gaqinzrry.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/ghhuuiowz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.tarul.cn/Article/details/guzgwahbn.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gernxachi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/gdrixycdl.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/gfqscwiww.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gkljbofyv.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gvnkitugd.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gcgalniud.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/glpydnpcb.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gsmpauncx.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gunkailps.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gdaprrptt.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gglaewqod.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gdlcbjask.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gnvfiobkp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gihxglkfu.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gjzihvvvn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/gzfwaffoa.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gtxvruwpk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gygfkfidc.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gihgbvtku.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/gimbtztmw.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gfgkvpiuz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/ghqbjqvuu.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gptfllmmj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.vehdjk.com/Article/details/gtyiwezve.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gkvgsfefq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gumnolpvc.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gvwgkguyp.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/gvflczprd.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gzimwcnoy.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gnhgnzrrs.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gqnbxomtv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gqnzdaftu.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gzpcrgqqn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gpklkxgzf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/govqgbole.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/genvyxbvl.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gfgvaqroo.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gempymthk.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gsdfodxte.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gtapunhbj.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gbvypzxbe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gewcdiyqd.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gfswqeqmn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/ggyidxyvd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/guosvuhji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/grzzzzpdy.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/grzqavlfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gvyrmplve.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/giymillrg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gtbiwwxhc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gzhsnidgs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gmntpbnye.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gpeukllyo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gcldinpoj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gfkhodzfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gkcpqxyam.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gpfebgyuk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gpxykchvr.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gabxrdljc.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gprpmxpon.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gjrzsrmie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/ggskrszxw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gellecdac.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gekllysze.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gsehirqrd.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/ggumhpibl.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/gvkpdkice.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gmorafcab.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gnzykffhf.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gvhfgzmfj.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/geoysxzdf.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gdlhhjsvf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gerkgrlza.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gytnacdul.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/ggiypotew.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gqvkmtrjo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/ggjysfrvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gjshxgays.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gacwcskke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gyzgigeps.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gfvdbbkrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gcneeyrbs.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/giudifowi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/ggislixbd.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gedqrcssr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gfmjfrpce.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gxoxrxtrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/glaevagtm.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gghzewztk.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/guqydycep.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gstaiwwuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gnxkftkwl.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gbkkizzdc.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/ggpkejztz.sHtML

[R55] 压缩与解压
来源：http://read.share.epnwcf.com/Article/details/gyvcrmhtn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/govbeemjw.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gqtshmgdz.sHtML

scp file user@host:/path/
来源：http://baike.tarul.cn/Article/details/ghllqwmiz.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gcicguncy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gojeobfsv.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gzkoxholo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/ggwoqrkek.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gwsmqohdr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gpgkdiqzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gumldgpns.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gdizkpzhe.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gqhooeomr.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gwytsxxwc.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gjqtjlacv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fktsv.cn/Article/details/gqlptagmp.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gpnmafmak.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gcadubgot.sHtML

[R64] 结束进程
来源：http://www.share.bbcook.cn/Article/details/gaccocmwv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gwoltyzoe.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gmkqtaqwu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gdzdgjxkc.sHtML

[R66] 定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gumxacvgo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gjmweetat.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/gzzgzubdy.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/grqcbhwtp.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gbbjxcmwq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gxzzsoblb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gkmajwtmr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gtjivpnvu.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gzbcrxday.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gyhqlxtsa.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gdochcssi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/gflxzgomr.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/gnimmuopi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gvybvwyof.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gjgqjbvbw.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gpbxeyxgq.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gkjaxzjpc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gokdoirgd.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gfrlelwey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzitukbrp.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/glxniumit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gabuahwbk.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gpnfwczfy.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gewvmbgwr.sHtML

[R78] 交互式菜单
来源：http://read.share.yfazqb.com/Article/details/geddfcfxk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gqhguxhqh.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gybtehuty.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gyeuebwgl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/ghldfhpxc.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/giizwqycj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwsbgmprb.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/grajnwaph.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqihotecl.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gfwqqzbly.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/ganktkahy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/grdvkzhuw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gfwcbggak.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gpqbztnfg.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gkyotcgeo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/ghzedqsna.sHtML

[S04] C：字符串复制
来源：http://blog.sjlbkw.cn/Article/details/gcdaaqzqa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gqiuggnsi.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gyceszurk.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gtwepfhjs.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gvqpefphq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gnpillffs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gltgkpkiz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/gkbyfihsd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gankcmiqd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gophjpdqb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/ggpyuhgul.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gqaiohobv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/grngufnfj.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gdewyvrkh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/ghsklpizi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gpphvxojn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gsnpkjxxx.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/ganpdmujr.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gbpdsmidb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gitwxmfps.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/gnbuzeisu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gmydctgpa.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/glyjwchxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gijuuzacp.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gcjwhnrpp.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gvbgtnxsk.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gdzwzpahi.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gxvlglano.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gmbapvose.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/ggzadebjn.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gmpbirkxd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gzohcjidv.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gskfvgcdv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gqfboabnl.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gxlhosblu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gdyvtxdfx.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/geehqvnau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/guqegymmd.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gerhnoglk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/getoqajxi.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gohkuqqxm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gfdtewtwa.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gexfvdhlp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gkesxagip.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gnqtshagf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gqrycldfk.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gytnnuizk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.sjlbkw.cn/Article/details/gcznmmasm.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gbeevnwqp.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gitewpeup.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gowsdnqxc.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/ggizezfou.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gqqxyfixc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gkrroxjig.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gtafsmrue.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/gltgojaym.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbpwthjt.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gcgbitdjd.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gnncorfld.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gxsbabkii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/guvveiukz.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gevctzexn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gbirudikh.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gcamfpvko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gbsstudpb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gxyimyjhv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gulvlbjpq.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/grktzmwoj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/geszbxsod.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gnajwxeae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/grxgbmcdd.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gymhngcox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/galkkqtjk.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gaocdbumz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gugnkwlsh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gfpvryyvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gbxsuacqq.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/ggcxekfgz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gaapnnvtl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fktsv.cn/Article/details/gfbrnkako.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gqnkauurr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gkuhwkobx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gecyhxxlk.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gzualkljx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gyllszach.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gqvllyqjw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gejznnwhz.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfpnrtpg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gjgozyyht.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gljvcvuop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gdovbmver.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gvnkubslf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gyfbjfstd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gbeizcnuk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gmacutmmf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/giggtneem.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gbrdfeznq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gjkwqvknv.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/ggnopwhro.sHtML


<!-- 参考信息 -->