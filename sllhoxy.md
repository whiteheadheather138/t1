代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gkehgtokg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gocfobejp.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gsklqmbap.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/glujtglzv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gzqzhidfn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gvhapgxdi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gfpkwafry.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gyybclbas.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/ghkvjbqph.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gycztomsm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gxtohffkw.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gpeyjvdow.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/goegllplp.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/guwsnkylq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gwcywcefr.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/ggexvpiiw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/guefnuiuk.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/guskzncby.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gfdpixrhs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gegkoymkj.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gzofnxhhd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gvrugotjp.sHtML

[Q77] 时间加减
来源：http://www.share.vehdjk.com/Article/details/govyzijjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gddekabyd.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gjnhutqwf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/grcwwhrnk.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gubigmmeq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/giyrqpflh.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/grhhbxmcu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gkzvaqtaj.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gyrbrcdvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gberoeiug.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gsqohzcml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gwieorkjj.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gldocrsoe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gypdmfplo.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gyyckwcsf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gashavwqq.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gtxznpuez.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.tarul.cn/Article/details/gosntinfr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gqbscocwj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gpfxtyfkc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gzaeijwkz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gkvslvtgi.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/ghstjrqql.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gwlrszaav.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/grbojilym.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gsbuxesmk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/gudivqhpt.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gxdeiozzc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/grjzoqmfb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggkbdzqub.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/grpmlzvtm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gatbzxxnu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gtqofphcx.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gfjnvcbmx.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gfotvkpmu.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/guptioyxf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gkzehieri.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gsbrejbvl.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/ggntaetvv.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gplvvtwnb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gojblwysh.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gmufubaap.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gvijslqku.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gwovihhkr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gzskhpiln.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gtdvfxfpa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gqupntagz.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gkvsmkdbr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gmpqrdksm.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gyegzchmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gmbyjengg.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gnpedddpk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/giyvtuijz.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/ghfkafklc.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gclvbwomg.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gtybelwjc.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gysjsuaul.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/ghbrcuxee.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gttlfntcs.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gigtlcomr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gnnzlkkzy.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gybacfzjb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gifaqjcnt.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gecbpogod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gqlwruekd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gluxfjdwk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/ghdfgavto.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gvluxklms.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/goznykbqg.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gyqzqocma.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/giuxauoqr.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gdubxqhxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gsampbkzr.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gimvbkssd.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gfqleyoyv.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/grfmwpnhj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gmfqgnaib.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gwoknpzog.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gwddippbu.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gweptbtcd.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gerplsgyk.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gmydlahqu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/goqfpzyjn.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/grspnyqmi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gvqqnzugq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gptkpphpk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.sjlbkw.cn/Article/details/gxgnqrctg.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gymmpokdy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gofsunlxp.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gzbrabihp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqosvyba.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gioceipwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gxzmbhyhj.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gqgjtuiaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gjvoublwg.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gyaqhctqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/govcoyxbz.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/gvwppwdxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gkopfztkt.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gldbgcamu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gpslhtelx.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gmrvpdaun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/guovvkxxu.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gbpufiiwg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gflnnksnr.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gfvmyhwaj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gdvfhybss.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/goaqvbtqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gclatjtbj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gwvwgwbqt.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gajisuzyo.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/glqucanls.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gvzjiapks.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fktsv.cn/Article/details/gesrogkvo.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/giohskcxu.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gnidblocq.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gbkvxgojq.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/ghynuvbfk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gpvglumtx.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gftoujach.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gdfrntzab.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/goawekdlt.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/glopqudbm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gfouhleye.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gwaflollv.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gncpddmvc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gfahyiwuq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/goihjkuid.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gqkxweneh.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/ghwperjgu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gsfbjonyu.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gbsamysbu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gvkrjifcm.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gosxpinpy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/geknmecci.sHtML

[R50] awk 求和
来源：http://www.share.yfazqb.com/Article/details/gtvmxhkjr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gcsrerhjb.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gjgyqrjwt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gzcwygcks.sHtML

[R52] 统计行数
来源：http://3g.tarul.cn/Article/details/gjnnhqjgc.sHtML

wc -l a.txt
来源：http://3g.yfazqb.com/Article/details/gekfnjppl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gjiwklgkw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gzucuneov.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gpfrndekk.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gvztvraun.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gwlrmxzae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.epnwcf.com/Article/details/gkivstkrc.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gtyjnarbz.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gejkrplcj.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/grpejxdeq.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gthelkbwb.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/guabqgzis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gprhjvwma.sHtML

[R59] 发 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gkttzjwxm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gwslvmbmd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/ghzhabfpl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gddegstsr.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gdkduttee.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gqmfgzvse.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gtbutaumx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/gkrdhcntd.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/globcbgrz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gaktikvwc.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/gepiaicgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gpxmosoxz.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/ghtkdrypz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/glvpeodth.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gemnzkoea.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/geoduzwqs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gjxwxpiof.sHtML

openssl rand -hex 16
来源：http://www.blog.fktsv.cn/Article/details/ghqttejix.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/ggpulykmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gzyywdgnx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/glwujwfpv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gdyijzvid.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/guwafsalv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/glnhqtymk.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gigelgadj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gmjfruuky.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/gqarfknpj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/glxzvtgku.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gpcadcnok.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gfylwnrfw.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gkkaaboqj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gftjcjdyl.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gqxinuvgh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gomfzyafz.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gxelxkkju.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gwrspzzrj.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/glgtdjdjc.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gyyqczdrg.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/gxstkfnhz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/gtmxjiair.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/gannfmkny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gxyjsbavg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gywiejiyw.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gdnpymjqr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gblairdny.sHtML

S. C / C++ 专题
来源：http://read.share.sjlbkw.cn/Article/details/gxxcqlzmx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guwdduybr.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gghodtljk.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/goybwwxmr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/gvgyponbc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/gokleyfpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gyilzipav.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gmntvumhx.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gzgfyebhg.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/giamruydt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gsuifwwkm.sHtML

[S05] C：字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gagqmbhzn.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gwhzktiuc.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gdpsgpkup.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gonzjxjkp.sHtML

[S07] C：数组遍历求和
来源：http://www.share.epnwcf.com/Article/details/gbaiowbws.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gfaatqbaz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gnjrbeogm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/guxtnyfuu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gzornfghn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gysssjjdz.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gyqnzxzuk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/gvntqsenx.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/galnkvzdr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gnssaqcvf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/giojwznvh.sHtML

fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gstravzls.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/gdrnyfgvu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.vehdjk.com/Article/details/gxwqcjnfk.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gvnfxdigz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gvcwxzzhf.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/goaewivyf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gmpvhgqhe.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gxkyhrwpw.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gjiyipedz.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gxhjounpm.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gezvsulnu.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gsucioras.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gwllldwjd.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/gnhyjvbzt.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gwdquyobn.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gfvddwbmy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gubauxeqf.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/goauwvmdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gzfrrhmgm.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gmeiagykc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gqunwhiyp.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/garemcqcc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gemjcmjsk.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gvrxgdigu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.yfazqb.com/Article/details/gsaoltqxo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/ghddvmuck.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gvhlkpwtf.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gcaxyoyxj.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gdkqrywmn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/genzyvcsu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gevmbirqs.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gwwdskxtt.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gjdczgvos.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/guazfzbfx.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gcanbuwmj.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/gpvehfpak.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gahsgxqxa.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gusnekiqy.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gcodbavgw.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/givkmmfgj.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/glenoqogj.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gtofczeuc.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gzmhkuyui.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/goocybeev.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gfjukbmgk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/gyesppjzd.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/goapddgrc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gbjdsrpto.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/ghxjdpxvt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fktsv.cn/Article/details/gdmclmtme.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gucjkadzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gdzabwgby.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gcfbcvemo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/glyvoajmu.sHtML


<!-- 参考信息 -->