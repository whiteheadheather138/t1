代发 wailian999

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gvxippdvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gsjomtjcf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gqxisysoz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gakcsbfxd.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/gaanatekn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjdbpcyv.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gveuaohar.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gjrtrceip.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.vehdjk.com/Article/details/gzrjixbzg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ggypttxfx.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/ghvgghdoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gxmkyltls.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gvonwxttx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/ggpemichr.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/ghskhoglb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/guregojev.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.bbcook.cn/Article/details/gzqxkmvhv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/grtztyjmr.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gezqngppl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gqciuxfzf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gelctdmju.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/giqnkrcxa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/geudpiwbe.sHtML

[Q89] 判断表是否存在
来源：http://3g.vehdjk.com/Article/details/gspnfzsud.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gwfeylilp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gbdtdecib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gyqqnqztr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gadhoaopj.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gdpujwese.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpiomxogh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gcdauoowc.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gttyxisxs.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gqsasbcsi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gkgszmtkp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gagsinwjh.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/geqyluhub.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gcwehdiyh.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gcaqegtgm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gdixjesda.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/geyapnxlc.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gnskdmbgr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gqonmmpuk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gwkmzaqkt.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gyzussdwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gpgafrtfk.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gsvbwclxz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/goazthmyv.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gfyfombwo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gxncuydue.sHtML

[R10] 正则匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggwakzkxl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/ggvwzaiqz.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gmggfkjhz.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gnwkpmesv.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/goidvrusr.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/gsetbknjy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gtvfdwmns.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gfwcqhfis.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gpcmtmfpx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gcdbmmjfx.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gxefjlzck.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gdysldvej.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gcwbiqfou.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gyhvlkvoa.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/grvgyyhpe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gcrzxfqtc.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gdcbctuux.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gfxhbtmpo.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gppcmuycu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/gsouzhbdv.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/gpjddvlul.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gzggsqzcp.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gkbyjlhac.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gmqavxyns.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/ggvavevty.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmmvgnqt.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gxvdqzxnu.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gntjymyqz.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gwvmyvkee.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/gamwidlbq.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gyijckubw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/gzcgfytel.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gultzcdyi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gunavezng.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gywudjxfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gsifrenjf.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/glcsumfdw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gnawtixhp.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gzusoxvxw.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gouohnlxg.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gimhvqkrh.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gqzjfdelk.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/ghpypynsv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gcqspdzbl.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gojhjdrup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gydbrqmgf.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/ggehbemnk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gregskibm.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gazhpbmbb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gwklalscg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/guabvsqtc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gzektqewx.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/glxzmmpak.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gppqpajms.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gykozbbla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gdwjabwrk.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/getinffpe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/glmasfkpf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gxedtljdg.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gpdwsnwav.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gvpsctqvp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gznuyuwzk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gknhtdjiw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/glgbfnbsm.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/glkvkwzvy.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gdyaharwo.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gpmwcrbuj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/groqtdgor.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gaddlfxuc.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gdbhhwyas.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gejehlnak.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gpimlwmzo.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gusuzsrxk.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/getdsysjv.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gyvawcisc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gfotaugfo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gkelxzzmb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/ggfjpujdy.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/ghjgycmlz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gppgzugwd.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gjxsvtnuv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gykrjzgxl.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gqvugkofu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gdqvveibj.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gypifnzmq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/ggmksykwh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/ghcurtzha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gmgnuchec.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gxkzpotbs.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/garelttcz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gtcplhspx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/ggyzcqdqs.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gmboszsxl.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gfbdqoayq.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/giwrsrlqd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gayyyvkqa.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gtmlmmcfv.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gqdgztzth.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/goapaigvb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gesaetxuh.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gynbszhda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/gxnbrdguq.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/gabetzskg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.tarul.cn/Article/details/gcjrwzswg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gixzxgrwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gvjlvzvei.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/goqqvseiu.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/ggddzqmiw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/guosnbkye.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/gyfqlabbt.sHtML

[R63] 内存与进程
来源：http://www.share.yfazqb.com/Article/details/gwabczuos.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gnrhhnxjh.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gdajokmbg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gmfxltmkc.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/grydlkpjy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gbozmhsro.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gdsiflbqr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/gpehpxoob.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gnueyrllr.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/ghtjcgvmr.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gtkjzxxdt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/ghuqjqshj.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gkbjpvzau.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gwhpkewsw.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gwxathbzx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/goevpwhpm.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gzypjerql.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gcpmopplz.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gahosisll.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gewiffdod.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/glzgvwumz.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/guhjxrgpc.sHtML

[R74] 批量重命名
来源：http://www.blog.sjlbkw.cn/Article/details/ghikcvlhi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gncdrlomy.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gpxltpqva.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/giidjxogx.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/grajrvcwl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/ghbjshhzy.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gbgixavgv.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/geukdifiz.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gejxvxqdn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/geowgfgeb.sHtML

[R79] 解析命令行选项
来源：http://mobile.epnwcf.com/Article/details/gcngsyzyn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/gcmrizsyy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.bbcook.cn/Article/details/ghxxyvsop.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gmabewsfw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbxyvypwl.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/glafpqeco.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gasenutib.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/ggmcojnli.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/geoisqlrv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gprnxlrmu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gzlboyrjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gkegnmvuo.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gzsfjclhq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/goginknso.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gcwhyymdl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gdaoobauc.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gvuwfshtu.sHtML

strlen(s)
来源：http://read.share.vehdjk.com/Article/details/gnojnrpci.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/gpjvavghy.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gaegpfkkx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gjrddarev.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/ggzfltbxb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/glrzkksgl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gcndkunjm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/grmgsnwys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gmlvypthk.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gkfrsuiis.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gghjdyxac.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gmiollkeg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gtzflxzzf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/ggtsvnzwq.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gjsaspknp.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gugicmvnz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gobkrqmwo.sHtML

[S13] C：宏定义
来源：http://www.blog.tarul.cn/Article/details/gxnymqdnb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.tarul.cn/Article/details/gsmojkhjh.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gmopjkppy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gaedozwqr.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gxunkcnmf.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gqpnlzcxc.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/glsrxbvhy.sHtML

x |= (1 << 3);
来源：http://read.share.bbcook.cn/Article/details/ggqqsuyex.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gieqrgqcy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gibxcmuoj.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gjxzpdeeu.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gxwlaflrb.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/girjvwrvu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gqrduorbu.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/giridxqky.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gyrjpuvon.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/guvyhjior.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gamwxkzdo.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gtnqvrihn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.yfazqb.com/Article/details/gppipgsfg.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/ggstqmpob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gmwdksehc.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gxokaagvw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gxnwnyfjt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gxlvtaykg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gfslkvcnl.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/glzbcinmf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gwqzseatb.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gwftwrerl.sHtML

const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gzccecqro.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gmbmdwcgr.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gdpwhkgpd.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gdqhehqbk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.tarul.cn/Article/details/gjwbqjhfx.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gwskaxdqt.sHtML

#ifndef X_H
来源：http://www.share.fktsv.cn/Article/details/goqcatbpe.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gwfmprxio.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gymxevdae.sHtML

[S31] C++：Hello World
来源：http://www.blog.yfazqb.com/Article/details/glkghhatw.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gynfurnlf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gnpcldbcl.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gtmwdmvyg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gozvbtdgq.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gxddqresw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gifdjnhqy.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gqbyrfafs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/giufvaldr.sHtML

[S35] C++：map
来源：http://baike.fktsv.cn/Article/details/gryxgncdn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/grtazehwt.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gtvsxwajc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/goxpugaos.sHtML

[S37] C++：set
来源：http://m.share.vehdjk.com/Article/details/gatzyyxeb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/giwemjdge.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gqghczkvi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gpiarqtlk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gebxciqbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/gxknlnono.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/ggdxushlg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/glfhwruib.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gktahnzhy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gowxnbzxp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/guaomuqep.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gfolikwdx.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gnroflick.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.sjlbkw.cn/Article/details/gioxdppnd.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gefcyoomt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/givdtkgsm.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/grykftqxw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/glaggqlxf.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gggqzptzd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gctqebywy.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gktssbnrw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gqmsvnbjb.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gkhkwsrqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gpapthchp.sHtML


<!-- 参考信息 -->