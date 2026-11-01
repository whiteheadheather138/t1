代发 wailian999

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/geogszyug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gemymnokq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/gvmxpdgcl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gvhedhwps.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gahbnmhry.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/geofhrohu.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gaguxezjl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gbptpebhz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gcqqgdgwt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcdkbzqmz.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/gummhkffs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.yfazqb.com/Article/details/gnzcrqgir.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/godqovcxn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.sjlbkw.cn/Article/details/gfweoredn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/gwloqyiyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/gyaojjleo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gazgidkov.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gcrbvtbzl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fktsv.cn/Article/details/glsaondfj.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/guqccuvmp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/guguhjjoz.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/grfofptmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gtlllkjik.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gozbrptga.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gmgbbdfqv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grsscojle.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/guvhafryi.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gvtxyonpq.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gusbuemre.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gzrlakgyv.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gilihkrki.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/ghqujwuze.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gcvafsoub.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gwstcptvf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gcwjesgnk.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gssaiqbgx.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gqbtljfuo.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gtqgtxrxg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gspmpwobz.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/goashscfp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fktsv.cn/Article/details/gmmwqozgj.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gvwyxqtje.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/glruvttqf.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gynudpptv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/guhcgyemu.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gvoamfkwk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gisuvexdn.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gkbayqory.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/goeubkvbv.sHtML

start) echo "启动" ;;
来源：http://www.share.yfazqb.com/Article/details/gesxbtque.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gnygufynt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.epnwcf.com/Article/details/gokhmkpuu.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gpgfyuskg.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/gcxgcvfuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/gwotdmraf.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gmuwqdsur.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gdgdasffu.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhjjyliu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gadzqmdkm.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gvspkupax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gfeaqrleq.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gedhudxek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gvatkfqkp.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gsyqusype.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gphnrrumb.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gzntgdpeq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/genayqyoh.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gylqgjmuu.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gjzvnsiwp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/grmatbgsq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gwuijgypv.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gsmslenud.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gnejagijj.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/grzbppjui.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/grxhwtxry.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gdvfbbfqx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gkhypaznt.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/ghsdpmosi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gthhbbfqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.bbcook.cn/Article/details/golqtoujm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gmjfabbcs.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gnynukgrb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/grkfgwcnv.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gshkkivoq.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/ghdyfgscm.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gyrkhtrvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gewtwwhxq.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gnnkkhldm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gplaftkic.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gonqkgfve.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gubwbobpm.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gcqbglnzj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gmzozojvb.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gatgtarwd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/glccrmccc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/gszkagnth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gnmhicubf.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/ggiodxpfs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gojjwwqai.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gnlmiqdlz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.sjlbkw.cn/Article/details/gydftayko.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gksnzzpmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/giuttqaba.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/geqabndzk.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gsindhipi.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gsqlgjzwj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/giorhtngo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gcnzjaezc.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/ggxkgehvf.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gzexpsmrj.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gywuerzzg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gvqagfjtc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/gknpfcear.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/gfzqkhppc.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gmayddgxe.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gqyytbdqb.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gjrfaksej.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gjsykdwuk.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gvqrdsjda.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gqybknlfh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gjgjbuhhi.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gcfiuwtsu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gxhkofsuc.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gmbbmtgap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gzzryqjrn.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/giceqknox.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gpjewcwjh.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gthecqfmt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gczxkryki.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gsxtzqjpb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gipzhuzwh.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/guwvgxsts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gvnietcjl.sHtML

[R52] 统计行数
来源：http://blog.sjlbkw.cn/Article/details/goqysqvdv.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/gciqtpkfg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gqmntihpk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/gnltcewue.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gjoxaegwq.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gnkgemcxd.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gvkflaapo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gadtgqfez.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gfsicysgw.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/ggqveritn.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/glilfowcg.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/goefnrlrh.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/grlmjjqnk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gaxjvqdfj.sHtML

[R59] 发 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gcdvpunsv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gbubrguoo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gghnztawb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gpjbbcyoe.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/glyolietg.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/goopzfjlo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gyqyzpjhs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gizrxyqhd.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gzggauqhw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gxmqbiuet.sHtML

[R64] 结束进程
来源：http://mobile.epnwcf.com/Article/details/grdclfava.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/geanzoymz.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gbrsotzdr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gyjmnwzvv.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gkljyafxh.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gbcfbcawb.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gozpmcrny.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/ghcnrlcfz.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gqypxyqgt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gvjdoedgv.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gmjmyxafw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/ghpbdmwvk.sHtML

[R70] 时间戳与互转
来源：http://baike.vehdjk.com/Article/details/ghhxpqacs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/geapaygeo.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gmwjaufcl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gpoyskijy.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gcrjvkmuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gsglfzfzs.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gymlgzssq.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gcadseofp.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gnigfrgzo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gcbnrvhfv.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/glmuukhvt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gvxgqbjng.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gscfsspjh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gkxmbbydz.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gdifeyntr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/ggiabemyl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gdixviogo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gudetdxim.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gaoodtjjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gmvxiqjxo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gepdhhkag.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gzddwkfpu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grifhkout.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gkgkaxmyu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpvuuygpz.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/glolwtyvy.sHtML

#include <stdio.h>
来源：http://www.share.sjlbkw.cn/Article/details/grxnsyoiv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gconxjsps.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gkuuszfcy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gpiabyrxl.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gzealumnc.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gvsnlreut.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gruifygsd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/gyrtumwhx.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gzcudreva.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gxcyhqnru.sHtML

[S06] C：字符串比较
来源：http://blog.bbcook.cn/Article/details/gkxpypqhe.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/geiaebhov.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gfeldmpdn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.bbcook.cn/Article/details/gfssbttib.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/glijqappu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gaskwyabr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gdhsyimbt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvvqsmew.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gilmpmlfg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/grtgpstiw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gshhvcidk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gydimhvom.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gbfelbgju.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gbvlpkaks.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/ghlcuewkm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gvxzxwldu.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gzedfuyah.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gqvsyzpvt.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gohoxertj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gltuciqjx.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gahvwspnv.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gwuvmhzhv.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/ggvzotyau.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gmdxxaxur.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gcpissmfp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/ggefgcatd.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gqzaualru.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gjruyazev.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/gipilhnkt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gveizdfft.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gkjfoezsw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gjxkeowyl.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gjyaekkno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gdqtbseby.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gblnwcsmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gfnybhgjo.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gyghaowfs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gsvrpabpi.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gmmddftfz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/ghkfvehic.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gpsyenbzf.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/giaabdbpm.sHtML

[S26] C：内存清零
来源：http://mobile.bbcook.cn/Article/details/glvojdxai.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/goupovcmw.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/geqbjxmdy.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/ghnftsfkn.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/ggcjvjdsh.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gtmswpwop.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gxoivnbhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gbnwmcksi.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gqvfgtopl.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gvotcjshz.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gqipiuwlx.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gudpuuhal.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gqjmdkuxc.sHtML

#include <iostream>
来源：http://3g.sjlbkw.cn/Article/details/gszqoeexw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/gkxvbefof.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gfthwyvts.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gqgnxymgq.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gkcowrrye.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gkvnwcoqo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gjobpgrna.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gbnalxrsk.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gdtdqcmha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gixzrghhi.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gnwduwcvp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gmubwqfiy.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gfplkvkjj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.yfazqb.com/Article/details/glalfqoen.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gwmkkvzow.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gexmlyfhv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/grzjmyfgd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/gksspkvde.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/grxjbketf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gtopdspre.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gojeilfak.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gqecqijgv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.yfazqb.com/Article/details/gxumrqidx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/gfudghoas.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/grdqxcsyx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gsmzuiwgl.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/ggsiwmwua.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gvbsouhrs.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/gnzqlousi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/gvsqzesjm.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gtwtyhnku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.vehdjk.com/Article/details/gpklhoebi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/getnfbqro.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gkobznynl.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/grsrowewg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gftbtmdfi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gtqjouhrz.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gilpgnioe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.bbcook.cn/Article/details/goezvwjic.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gcojlrley.sHtML


<!-- 参考信息 -->