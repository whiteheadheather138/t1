代发 wailian999

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/ghlgwscoc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gqqlppkbl.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gqwwthojf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gdsorihqt.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gjmpsafmm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/ghwgkophf.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gizjypniv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gdueahffy.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gmyhynsvb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnrjhqrhc.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gbgkovhay.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gpzstroeq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gmhvapwmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gsamcqagb.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gibrclnsw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfnqlaetj.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gvqppvooh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gadnjisnn.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gmqzyeqcg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gbetkaizn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gqxfloygr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gixbrdecz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gjnoxscdp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gfxehicrf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gdlejmuqa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gqchxbhwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gcerglfec.sHtML

[Q89] 判断表是否存在
来源：http://baike.vehdjk.com/Article/details/glmcagqfw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/ggxtamyoj.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gikczcdws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/ghwnlfdas.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grjrhrqjf.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gshcfotee.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkhzkyzds.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/grjzxdbqh.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gyqywjqri.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/geohjmquh.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gekdkborh.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gsjjplvpv.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/garxkhmkg.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gtwdifyab.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/ghllphciv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gademzbra.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/gxtcdcyod.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/goknasmlp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.vehdjk.com/Article/details/gqpgrupqc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gsfmtzcud.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gjqqggzvc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gsztflvjs.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gpujikhlw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gqoimugnz.sHtML

[R09] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gnqaksahd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gzpoorfnn.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gwfrlbwun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gmrmekbqm.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gskhxsdrh.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gfkydmlut.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/ggyychpgs.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/guzcufnnl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gxhhrfhqp.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gzwviqsnb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/grcwcixwr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gyqzedbzk.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gwfkvuerv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/ghblotixp.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gtzecbgmb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gqvnvarwa.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gledmtovs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gjzgoyeit.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gvyhrhfip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gnjuvcrnr.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gonduwwul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/geopigunk.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gbtskiqxj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/gldmyvmyl.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gzbcguzru.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gbytuufgj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/gmcthixnh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/guigjdwav.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gidrflmro.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gsppupyek.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gcmmhllae.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gifksicix.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gwuqnmxes.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gdhspjnol.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gydtrympt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gdortjdyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gkgprafbi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gjdylqlji.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/grihlbttv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/guuqroznp.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gbthehzhp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gmmovtvsa.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gfprrzpyx.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/girqdgbms.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gltbyomgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.vehdjk.com/Article/details/gnuqncgcw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gecwymlko.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gyurffqgy.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gilaarmyi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gsyscgoqs.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gplurmaav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gczqgfrbo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gzpdynisl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gtxaufcxw.sHtML

[R34] 退出时清理
来源：http://3g.sjlbkw.cn/Article/details/gixxjtmkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gwsmzossp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gzclgjueb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gyrbplknd.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gjyvsfnts.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/guxksqbmm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gnkpfxowz.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gidnnouet.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gmkobtrvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gznpmzrgj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/gpdpkkzmq.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gtuksfzxj.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/ghmsuhvnv.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gmfkxwpxl.sHtML

[R41] 丢弃输出
来源：http://baike.bbcook.cn/Article/details/gdrfjvlqg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gbawhoocz.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gofxpemjv.sHtML

wc -l < a.txt
来源：http://www.blog.fktsv.cn/Article/details/gkgrohczq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gfywdwkmv.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gpcpiyntm.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gyzvvntfg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/gmlwcrwsl.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gmaplagxz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gbaywdzok.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/gnnxbvgjx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gpwsczwnz.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gwcaokmye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gdzjkdckg.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gcbbocbmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gaqokgzoy.sHtML

[R49] awk 带条件
来源：http://wap.sjlbkw.cn/Article/details/gqdwoxzvu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gawndxwlt.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gedzgrfoa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gijiigfof.sHtML

[R51] 排序去重取前几
来源：http://3g.bbcook.cn/Article/details/gafgnlpug.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gnzvjbpko.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gptxqrown.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gqqztgzkz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gvmsjqdta.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/gfadgeyyy.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gczjjadwd.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/guztzvwbe.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gcfyvooip.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gulqdguau.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gfxtbtfek.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gzcaiqcor.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gdrtnerjz.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gorsiuafw.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/goolekhtl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gqvmlbana.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/godjonexi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.yfazqb.com/Article/details/giznhyowc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gxamcepub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gwzltsaaa.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gmsgbdway.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gcmviiyeb.sHtML

[R62] 找最占空间的文件
来源：http://3g.sjlbkw.cn/Article/details/gcucvlqkj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gdrqyxkdb.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gfkuemtuf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gqtdgeyrg.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gqhhmtcgn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gkhtijmwf.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gwbxzlcpu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gzojgzlkd.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/ghbgpkeiz.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gtfsejext.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/govpjbdbh.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gltrrxusw.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/gnkxmzyau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gxedwuwfu.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gogxdwpjs.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/giufiwobn.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/ghmvqqdeq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/ggyaotsqw.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gxhrervdv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/ghnsrpggk.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/genpfigxh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gilgnizur.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gqjrvscmh.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gmphykdsn.sHtML

[R74] 批量重命名
来源：http://m.share.tarul.cn/Article/details/gmanyzsch.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gqrgzbqem.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gbfdfaxsw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/ggiqmjsja.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gcnvdhoji.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gjnnedrqi.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gmfwjmydx.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gwqhbovly.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gqomyuemw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gldnrksfw.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/giealuqhq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gekofjzzf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/gvxiarfbo.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gvysvlzcs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzewypviu.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gjplrfhto.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjbbeyqev.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gqtevbvmg.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gtmcuoash.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/ghinvvugk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gijgmqlks.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gkbfiyyoy.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gxnvtmqug.sHtML

int x; scanf("%d", &x);
来源：http://blog.yfazqb.com/Article/details/gboztigvl.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/ghhbltwlp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/ggmclwuce.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/grplomvzt.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gzjpaeerm.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gflsunufe.sHtML

strcmp(a, b) == 0
来源：http://www.blog.tarul.cn/Article/details/gweftbluu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gftioyaoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.bbcook.cn/Article/details/gtkfohlej.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/ghykvmicp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gpcnjzqye.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/ghgcgiouw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.yfazqb.com/Article/details/gdogslwbc.sHtML

[S10] C：指针与解引用
来源：http://m.share.tarul.cn/Article/details/glfzqrfgc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gsqrlalux.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gcfmotyda.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/ggjuamzer.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gqgkacxvo.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gsejrfxec.sHtML

[S12] C：写文件
来源：http://wap.fktsv.cn/Article/details/gtnxunptc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gjoynxood.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gkpatbbxk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/getkongpu.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/glydmipgr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gthbljwuq.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/ganatrben.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gafgoglai.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gzeuwaysd.sHtML

x |= (1 << 3);
来源：http://www.blog.bbcook.cn/Article/details/gdpkrsxdh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqvndjkgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/goskuquhm.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gakvctknd.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gxnyrflql.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gscjugbqu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/ggaykfsyy.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gjscbmsou.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gbponsvks.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/grrfvypdy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gvgbujivu.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gforhuxml.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/geggqpoos.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gwpcenynl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.bbcook.cn/Article/details/gjxrwlval.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gshngzkfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/ghnwczaey.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/gnmjdqruu.sHtML

memcpy(dst, src, n);
来源：http://wap.vehdjk.com/Article/details/gaawpfxtn.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gzupwmglq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/ggdrrjxug.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gspwlkllu.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gvgsymfxw.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gmdvgptln.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gjinagfjo.sHtML

[S29] C：变参函数
来源：http://wap.fktsv.cn/Article/details/ghoptywfp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gonmqtnfo.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/glwnnywaf.sHtML

#ifndef X_H
来源：http://3g.tarul.cn/Article/details/geqyhocqz.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gypvqjcgm.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gxmnlptsb.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gcowhavzh.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gwxahpdsp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gktebzzia.sHtML

[S32] C++：字符串
来源：http://read.share.fktsv.cn/Article/details/govfqaias.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gfzomasvz.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gygbmbzcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gldoxmbrj.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/glivnbzbs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/girnurlpq.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gmmtzbguw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gwbzgnalp.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gczleaylp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gyrhokjly.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/ggllakenx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gxmkloxyg.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gaqjhruyf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/grsnqvekr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gcepoiocr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gnbvdyeii.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gslbonnxw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gdrfqinhb.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/giwkcpeuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.sjlbkw.cn/Article/details/gdugsqaqd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.tarul.cn/Article/details/gllwqutof.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gdsvrlyad.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gfccehpoi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/glzsjrxsz.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gircjhrer.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gontdrygg.sHtML

[S45] C++：lambda
来源：http://m.share.vehdjk.com/Article/details/gxaskjthy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gjrvqyvoa.sHtML

[S46] C++：函数模板
来源：http://baike.bbcook.cn/Article/details/gjwwvjifs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gevinnkgq.sHtML


<!-- 参考信息 -->