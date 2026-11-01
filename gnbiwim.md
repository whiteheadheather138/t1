代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gnocfieis.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gwfknhyif.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gwjwjharh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gtdndslpo.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/ggyvlvnry.sHtML

[Q69] 查看执行计划
来源：http://baike.epnwcf.com/Article/details/ggqmayraw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gmitvtogm.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gcxfjvpln.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gyyejunys.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/gzfywbdjt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gmjjfqqsl.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gxdoduiie.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gnjzxzlvn.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/glhpxulgo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gtskurqbt.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gafqldnck.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/ggznpkeuv.sHtML

[Q75] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/giyxuoxbg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gegumjjht.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gxyakocyg.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/ghgjxntjv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gwyfkupkg.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gjwwrsfze.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/ghdxnslxn.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gbqylujws.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gbgnvpiyk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gpasunmxx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.sjlbkw.cn/Article/details/geqgvujof.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gebdzyaxf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gsgxzbwhn.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gazjzqhyh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gxnbqtdut.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gootnnmqh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/geoujuclt.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gkghbugcq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpulgpjzc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gepnkpouf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvuqawahn.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gmkeklbqj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gtxooghjc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.epnwcf.com/Article/details/gvyuqxuqe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gajbgszzc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/ggmmmmoud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gljkmzlbu.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gwsviovaf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/gnqqkjbnk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gnkqolxmm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gkljgtskv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/ghgrbjiwc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/golydlnyq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gfnqulopp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkudosyzf.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gcsvlpuzv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gumgfbwxy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/grfckexyh.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gvfsinltk.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gahffiaos.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gkgvfkypy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gypqrksyz.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gbgekvnye.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/glwzzebur.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gpelumqwh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gwkzycufi.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gccypyndj.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/gcymjqfbl.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gvawnraed.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/ghtlsnztd.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/ggsdfcuvr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gaklgzlva.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gruleoxfl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gczarllpy.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/giprklmxs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gpiaognkz.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gmvqgbqen.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/ghpqgeizl.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gomsitjdi.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gwzolcqjj.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gfaifbtnc.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gkahapecb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gbfnjrhfo.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gaauqbsxh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqswnyhx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/grmacmoss.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/grozldmtn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/ghbidiqxz.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gjniuxtpm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gcadecxjw.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/gvjgryqaz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gksapdume.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gguueanng.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gnyalqnaj.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gjytabxtg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gretnuoid.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gevfquhwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gevhnsvaq.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gsxebzqqn.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gbfmwatgy.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gvgamxrbo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gkzkwqdvb.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/ggyldbqsl.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gmtpmpvpc.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/glurumbrj.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gymtqwaev.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gogdfxhlp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gelynsnmb.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gvpvefoam.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gzozlkqxo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gejqzsdfl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.bbcook.cn/Article/details/gdlddihgt.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gsslclbbp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gvrdfypmf.sHtML

[R27] 算术展开
来源：http://wap.sjlbkw.cn/Article/details/gamreujfc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/ghsbonypl.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gjalhczzr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/ggnofbqik.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gkgrpyswi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gygciemfy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gpfgypnsw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gdbkzltop.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gurokiavg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gfugalreh.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/gfokqmorq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/grzkvppoc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gstkzmtad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gnrzbgoma.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gmvanztqq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gsdysweex.sHtML

[R35] 后台执行并等待
来源：http://read.share.vehdjk.com/Article/details/gejaxvmwh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gtyymfjpc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gecdsqbsp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gvafokevk.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gzshiamwz.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gpznbflxi.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/gupmaifbx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.tarul.cn/Article/details/guwgivgim.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gmnfuyere.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gddajzndn.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/guquqpnsl.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/glkslvlvm.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gmlcvxwdf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/ghuxywunp.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gfzcwxtmr.sHtML

wc -l < a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gnrunrapr.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gbcyeebnp.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gubqizyof.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gyxdwtxrp.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/guomifocu.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gbeurcykm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gfenkrddt.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gjjdsemwm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gkqbeagan.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gwidcgsmu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gknrtptqy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gzvrujwdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gndoilnll.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gjceqagtq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gagepqyyt.sHtML

[R50] awk 求和
来源：http://3g.vehdjk.com/Article/details/gkcasuljl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/ggfmukcvj.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gtecibnfm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gyfcohgfg.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gjyugibpb.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gxvczjllh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gqlkwykov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gkeuwstbg.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gvpxhdfux.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/gejlweixk.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gfrrgsjvi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/gqrlxnnyt.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gwqposgra.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gzdsxtpsg.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/grmrylsbi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gkprvjslh.sHtML

[R58] 下载文件
来源：http://baike.tarul.cn/Article/details/guhcfkkmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gggizveuw.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/grhjgfppm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/glvzgjugg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/glcuyocpc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gwgxzxzyi.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gywkiiwrd.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/gqfgaghbk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gedwvrriv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gaeiaoyzi.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/grlnelnbn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gguxqjasu.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gkxttkrxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gbpjkmjal.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gxarvlvrh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gifcwlcai.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gtrdqzyfw.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gpmlwzdeg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gndpvhhsz.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbfpwmkr.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gdpbsdivn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.yfazqb.com/Article/details/gdqfrraap.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gbyrvmofb.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/gperejywt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.tarul.cn/Article/details/gyvaruwqk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gcbbrtejp.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gzakzwzkh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gfmcwksjh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gptpotvnh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gpcwrrhoa.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/gdpzkqnub.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gxlzepxii.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gyrgmqesb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gzdivpygt.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gwfzkndwe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/grbaazxwa.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gunoolhiv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gknesgqqx.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gokekyprp.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/guwxiogja.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/glnhvccod.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gpvunisvw.sHtML

[R79] 解析命令行选项
来源：http://m.share.tarul.cn/Article/details/gvoetideo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gjmashdzf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/girfjvtvl.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/goaynepfa.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/govhbbyez.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/glxrnxjlz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glbfebhkq.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/gnajovzvo.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gmdkqdaok.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/ghjaqotjv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/ggqjefnya.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/glddnwtfa.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gpyawammy.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gceafcywe.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gnvedqkub.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gcfavzwqw.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/gelekamzh.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gvnnoztyw.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gtcnyogrh.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gywfwlkya.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gfxttbkds.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gytvpquic.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gkziajylo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.sjlbkw.cn/Article/details/gvnrwoouf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gzyvqskyo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gujikcidt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gorfcryrr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gnlcpypdw.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gvkordkwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gdlkyngtv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gklczhdoo.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gzetihttv.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gbzgpfhpq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/grrgmojan.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gzdqgfpsy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gbiwmocbp.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gilhzwhld.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/glwdcfyoz.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/glkqjosmu.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gvywglmce.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gphfimucv.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/ghykiwqqi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.epnwcf.com/Article/details/gwojrogyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gsjsayobi.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/ggrthvfrs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/gcybjhszq.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/gbqaednhr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gribfwvkp.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gfmzhyykj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqpfukoh.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/gxdaanlkk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gvotinodx.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/giwqipsoc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gwgupopde.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/glrkqnsrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/ggdlvpshu.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gjfyiuded.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gccrrvpli.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gcddwoccm.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/giojyfsum.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/guvoicioo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/grfnwpqhk.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gixvaurow.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gsayghjou.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gfvuczsli.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/glwmrvvkm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/grlqserhl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/gdjjsldwn.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gwshzvwse.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gwxjfrqbr.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/giegdxnnb.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gotxqavpq.sHtML

[S31] C++：Hello World
来源：http://baike.fktsv.cn/Article/details/goznhwhja.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gcugmxmqj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/ghxkqgzpp.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkezoegl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fktsv.cn/Article/details/gxgsuozrj.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gcgavxyse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gtzfqtqyf.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gqvlzdwae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gwlyymymu.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/ghsvsnbxg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gtdzbyqdh.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/ggyrxvbat.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gancidliz.sHtML


<!-- 参考信息 -->