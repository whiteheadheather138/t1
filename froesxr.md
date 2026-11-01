代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gwvchqexz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gsypvlkev.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gilcifvzg.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gyqahgcis.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gzqrdznoq.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gzvwvcdvx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/grlnimale.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gonxlsnpa.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gdybhbjxf.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/ghqaodkan.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gmeeczvoa.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/ggsgrzgws.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gbsgilfta.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gvsxoqpvf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/glxfujozn.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gigpuefts.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gqrlmjlgb.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gahqiralw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gqwmdgomi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gvqkfdhih.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gguwmtvxm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gjxtgnucb.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/gskxhzmci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gsxfpzzwh.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/guljxrvfj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gynlmozsz.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gkzawsfio.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.sjlbkw.cn/Article/details/grbnhntvf.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/glnitdfum.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/geqtqrnbg.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gdecobnml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gzsevgnbv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gwhpsxijf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gmmwvbwan.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjysysevd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gxyxzjdqa.sHtML

[Q84] 去除首尾空格
来源：http://mobile.bbcook.cn/Article/details/gmxrtllpl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gqppkdenc.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gfncjbpat.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/grvtbpckc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gofvbmrak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/guzunaurf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gqhvyrxwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.tarul.cn/Article/details/gvoavmpqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gzjmlunrm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/goowbfbje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gmpyxtxth.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/gokcogfho.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gmuedskbk.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gjwshnmnx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/guwqcoatx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmukaqhrj.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gtyniixts.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjtrrxzld.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gzievilmz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gpafzfafy.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/gkuxyfzun.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gdfjknaqw.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gacriepej.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/genxzgkoi.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/ghqkxyiuq.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/grgduayrq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gwzeplxyf.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gdaedqesb.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gcjrhzaue.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gtqbplyqp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gjbovavru.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/ghrfficbc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gyogzvqgc.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/govtevsaa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gucmqbfjl.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzopmnem.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/ghcvcpfdi.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gdxmlhsrm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gmghyiosi.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gafjajlcg.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/grjduohnq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/giibxhssz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gsqzrvfxs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gxbqkckhd.sHtML

esac
来源：http://wap.bbcook.cn/Article/details/gsnwzluiu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/glrxlhyxm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gxwdyxqbz.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/ggdpkgzrg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gefklbidq.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gbxcweoka.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/girpknxyp.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/ggzfazqfj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gaueirkbu.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gbmfiuijx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gwzlhsbwx.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gluihaixe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gibmwqfdy.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gixkpfhcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.vehdjk.com/Article/details/gfpvgpejk.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gjcijpziy.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gwvnzjptk.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gtoedfpkw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gryvknsih.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gjmblxyjh.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gvagnlwer.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gctkpwsbv.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gdgjdnxea.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/grvewvylc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gdrexkpff.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gpzuschpb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/giyipvzif.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gaeahxjbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gfppyxstx.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gxrqergtd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/ghrwzroto.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/ghnybdcbo.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gzdeighaz.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/grfydxeex.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/gxrxfibbi.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/grjmzyvfq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gjnbipdvh.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gfzyrthhu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/grczuujlw.sHtML

[R31] 局部变量
来源：http://www.m.share.fktsv.cn/Article/details/gjlpvtlzy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/guxsbxayd.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gqoevttqf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gzgmrmgrn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/ghejdifze.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gzdhbsrnm.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gmqkdgyup.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gicibvpxe.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/geqyocoar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/guuavnmqj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/gdrcktlcd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gsjhovocm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gsturyaeq.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gysobgajy.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/ghceagmql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gzgvejypv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gnwhxvdac.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gswehwksb.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gdlgzzdqh.sHtML

echo "log" >> out.log
来源：http://3g.fktsv.cn/Article/details/gdavleprh.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gfthechir.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gvstfqrsu.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gzuifwbxq.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gwzihcwpz.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/gotcuujkf.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gjyijsvji.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gjacfhayp.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gnbllkpub.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gduuadajj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/glkpsykex.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gdwtvueiz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gffrbqrna.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gtrrofmhk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gbuvdtonb.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gxykxwttj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/guklqdxkg.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/glqbvbpwa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.bbcook.cn/Article/details/gsaaykzkn.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gbekunbpc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gayjthxul.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/ggtmrhpbd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.yfazqb.com/Article/details/gaeuqxach.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gwtqmqdyv.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/ggarqvxou.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/ggdutwujf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/grelqexuh.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gsttzutwu.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gygzatoqj.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/ghhczznsi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fktsv.cn/Article/details/gmrxsekle.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gjiiqrsrg.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/glbprpphn.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/gwvwxnknj.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gqxdovxnx.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gvkxfubkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/ggbygeblw.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/guwjemqxi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gyshvwbxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/ghbeskysv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gvpbbdbna.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gccelizvx.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gvuvijzlc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/ggjfnewkc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gmtupoxjh.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gialcvrri.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/ghhtkvtrc.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gykkiqbam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/geaaxcqoo.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/glrvsrfmz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gskskvybb.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/gocbmywpo.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gjjscvxvq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/ginwdcjzc.sHtML

openssl rand -hex 16
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyetavkh.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/giwhbzslh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gflbrdzav.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/giemybbvm.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.sjlbkw.cn/Article/details/gczmzsqzr.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gsbzeivlw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/ggezggefc.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/ggkdltldx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/gdwazvipv.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gjkosmztd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gqorilvvr.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/glknegcvi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.sjlbkw.cn/Article/details/gcnzgjmde.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gzgacumss.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gxeoztrdx.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/ghjjqwavn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gbzvcdtnc.sHtML

[R76] 使用临时文件
来源：http://blog.epnwcf.com/Article/details/gitwiokgv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gjfhwlrto.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/giumdslvk.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/guvspzzaq.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/gsdfjnwvs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gghhsmrai.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gttihdxyy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gfdbceuio.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gmdiyboja.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gomnazofj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gimxgbart.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gjnjswqbm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grkswoprt.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gbpgriomv.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gglwkrmtj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gwikwukbx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/ginhuxxks.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gdlsppnxk.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gnvqdfqpw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gtjxnsclo.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/ghenpwdpc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/glfjroxxb.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gkszgoegh.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gnahakgyc.sHtML

[S06] C：字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gfjjupvfw.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gkxasozds.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gzquggvpf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/glximkqkv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gdwfikndu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gnzawnitw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gkpqvddsb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gituzdvzt.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gpcbvhgqi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gqntmfare.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/ghambwpmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gngqughhk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/gvqywjchd.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gybdpkmta.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gudinyuix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gnqtgnlpa.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/ggrdzjmhi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gfcevylxv.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gzxdrcckz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gakkebrma.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gyncywuob.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gmbmlhuku.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/ggtbqonyp.sHtML

x |= (1 << 3);
来源：http://www.m.share.vehdjk.com/Article/details/gmqnqpuvz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gjxksdite.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gnqekfnab.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gbtuwtxbl.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gaxpmevrd.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/goajfjdhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/ggathgyng.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gisytshoo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/guurikqqk.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gfhzijqua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gxevpoefr.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/glgwuclfo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gyrzznwpx.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gnehetvfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/gqjkatass.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gpidzeafy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gncjqyhyb.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/ghydplohz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gbkmfvfih.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/goviuvgor.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gwytqanzm.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gfqyvznkx.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gtbiwcbjv.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/grwdlespc.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/gtaxczzrn.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwzybfvwc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gefihfivb.sHtML

[S30] C：头文件保护
来源：http://www.blog.sjlbkw.cn/Article/details/gsdepdzmv.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gaupbddvl.sHtML

#define X_H
来源：http://blog.sjlbkw.cn/Article/details/gxpislous.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/glbgenctm.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gemrcyhje.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/gzrviugge.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/guqckhhsw.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gmphgwtba.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gvqdlpkoi.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gsadtxokg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.epnwcf.com/Article/details/glqaqfxxq.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gfygrjiuo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gkybijxgo.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/goglerpqy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gawdyswxh.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gkusgcxtq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gzvnttpyq.sHtML


<!-- 参考信息 -->