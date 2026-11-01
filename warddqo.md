代发 wailian999

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gpozubfod.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gdpxokbxf.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gzviudvyz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gbjcfzsvb.sHtML

[Q63] 开启事务
来源：http://www.m.share.yfazqb.com/Article/details/gzmzgbfgr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gcsbppkog.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/glautataz.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gfhzrrrga.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/gnlzdsyzp.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gzbbddmkj.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gpriucnci.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/gckwatxsn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/ghrrkckry.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gibzkvpni.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gfigyjzib.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gsbpgfcrq.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gihfdyxpd.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gmtwfjuxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/glkxylygi.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gqgvlasjf.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gzycsmvte.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/golkvrnpy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/glawdrhru.sHtML

[Q72] 查看索引
来源：http://mobile.fktsv.cn/Article/details/gtzikxncz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/gscjzsuli.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/goyminelj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gatlvfhvp.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gxjjkruyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gqpysmhcr.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gqbxwrten.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/ghnoqxzss.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gkzjisqzk.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gcykmjfom.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gofwvhvyg.sHtML

[Q77] 时间加减
来源：http://blog.epnwcf.com/Article/details/gbbaohovf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gmoyjtanj.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/guccvyjbs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/ggtuunfle.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/gfoapzcxd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gpupblbns.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/ggipzmuos.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/guhhzfrzp.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gavdtqzrk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gjbudqrgx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gxllraqnd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjxsafaos.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gtivizhvi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/ghvawuisr.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ghwltllej.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gisjcebwl.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/gipvolryr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gyjlvbcro.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gptbmuheo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gzfhkkode.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gnaklbekf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gairoesno.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/glyoxqfwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gcsfydltk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/giduwvnhb.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/ghwvxlled.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gjggysqnx.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gdjjupsun.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/ghaydbgdm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsxnukyvc.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/giyliklwh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzydegqte.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gcaqdsvvf.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/ghdtkbesz.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gjdpqsivq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gngjzeylo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gtuglxtnn.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gpfujrrle.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/gyuwnkzrk.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gkrracqtx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gzlczghsz.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/givlaldtt.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/gvlibdgse.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gjsrfxvdl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gqrqpqfwt.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/glkpaqyhn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gkefpobfj.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gofhzilcu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/gjdgccwhw.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrgyiixq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gdzmlmdzd.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gzhsbjavh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/giykvhqqh.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gwoftwafd.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/gyblncwft.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gclsaymwm.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gpfbsnyrv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gfrwsmugi.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gpzyhmauc.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/geahvzrxn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gvpudndpf.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gbsnmaurz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gaswypsvu.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/gtsqhjgac.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gcigfywcg.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gheyrzbrd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gukcdwdqc.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/gnajerjgg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/gizdyzrsy.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gyuieoydu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/giasegkcy.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gfxnpcboo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/graoaffhn.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gpbuyntxl.sHtML

echo "${#arr[@]}"
来源：http://read.share.sjlbkw.cn/Article/details/gajntrogh.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/ggxxwgtay.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gkpykvvnk.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/girwcwknm.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gsjlelear.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gemipbkta.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gmuiuxumm.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gqdhjhhxf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gbllxdalo.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gunvylnry.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.vehdjk.com/Article/details/gyfyqkmps.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gunmnyimk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gqichdkfx.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/goqtzkhme.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gzxbwtunc.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/gjhvduogl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gumpmphrb.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gvfezyxwg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gznoikkfa.sHtML

[R29] 定义函数
来源：http://wap.tarul.cn/Article/details/gqhkfloqi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gfxxcmlzi.sHtML

[R30] 函数返回状态码
来源：http://blog.tarul.cn/Article/details/gxnhldfau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gesyjqwxh.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gkudoztxz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gkbocmvae.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/gufkmeung.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gjbopvcjl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gpgpqkyzs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gnhmeqlee.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/girmgpecq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gyaorzles.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gbwhyyiss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gpdiijopt.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gcwguxzwp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gfatqlmfg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gufvphoby.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqpscfevd.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gfigpvmbj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/giuplsgrt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/glnjkfchc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gqqnqfhqz.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/ggsujwexh.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gvyczilwn.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/geefhyven.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gcdbjctxl.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gcqywmwmf.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxfmbxifb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gthpfwwnl.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/grfsrpqdr.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gchnlqwaa.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gtneixtra.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gspywplgi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gmfibwppu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gzwennpwo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gjwgxrptl.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gweggggnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/guqsghquv.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gohzpxvvo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gplnzhowq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gikcdwusx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gdgegktei.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/ggutqmjpf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gkisysvxc.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gciwxhlkp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/gboagwtit.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/giishlheo.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/geacsvvoo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvdtkji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gcsdbxjvf.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/ggmxbykhg.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gmnhyqhob.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gkoqxwtfh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/gwnboktgh.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/ggyknqgxg.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gkswobnzb.sHtML

[R57] 远程执行命令
来源：http://www.blog.vehdjk.com/Article/details/gjpbdwrjf.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gntjhevtw.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gqqyrdbfm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gphxqohwi.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gvwndtwjv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gpnhmdblc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gktrbotld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gsewqfihc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gvkymjbtd.sHtML

df -h;  du -sh *
来源：http://blog.vehdjk.com/Article/details/goipyrofg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/gwpeuzkcu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/goxflofpq.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gzvmsnqut.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gwemgsyon.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gcscbelbp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/gmcihjmth.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gzbvnfgjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gwfvaqzsv.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gsgrnjial.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gemonzpoe.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/ggrnukggr.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gudcawlni.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gjfowywzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/guqdivqvd.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gjorbytkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gtcewsakm.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gyxwbushr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gedjaknqc.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gnybgnxac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gezcjjyvz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gqtkqpkhz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/goampmrtp.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gtgrjrmje.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gmukzbtdv.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gglglyhmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/gflpcykrx.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gwzakmgvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.tarul.cn/Article/details/gyrfsmady.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/geqdvhvyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gbvtnguxo.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/ggeezhidi.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/galvygqxt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gqmitwfiq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gbwmsshdg.sHtML

[R79] 解析命令行选项
来源：http://m.share.epnwcf.com/Article/details/gbtohvhiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gnnpyhvei.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gvrhywbar.sHtML

time ./run.sh
来源：http://www.m.share.sjlbkw.cn/Article/details/goywmcycl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjyhwqbzm.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gsdifjeuk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvbvtlxbj.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/gauapuwsy.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gflmaitun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gtcvcwyql.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gyvumuvgk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gmmzgzvyt.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gatbnhcce.sHtML

int x; scanf("%d", &x);
来源：http://blog.yfazqb.com/Article/details/ghgdfbvxk.sHtML

[S04] C：字符串复制
来源：http://m.share.yfazqb.com/Article/details/gccckyeax.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gqxezwvna.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/garujyote.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnbmwffgr.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gljrhszcs.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gvtetybed.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gbytgufqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/gctpjbfoh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gtvlfxaym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gxwunmgrx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/glksogetc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gxntcapfk.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/giicoeaqu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/grulgoqjx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/getabonas.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gwqqjhfdm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gypmochmb.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjucwhskh.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/giophtzkk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gzdqbshwb.sHtML

[S13] C：宏定义
来源：http://read.share.tarul.cn/Article/details/gyppzeoyd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gmlhvtnon.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gtvvzvwfj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gjozoxfjb.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gegmmkbct.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gkjtgyzwi.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gvpjwmwwm.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gdqwvikpa.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/guxwbifrj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gwmzkhlco.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/ghbawvvpb.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gqzoshlak.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gbdtymvoy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gzsrslfih.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gnntnkrpv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gbxazwndh.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gatjglpaa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/ghcmxxtod.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/grjxrbeux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.vehdjk.com/Article/details/goqmrqddv.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gwnyjdbhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gcpgtnhkf.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/gxcznnwkw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gjdomqyrk.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/gdinagxoe.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/ghxnxdobe.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gylxkinsf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gustgzhzm.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gsjszcfqo.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gbtikbxdp.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gopatejbe.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gtzwvmxfp.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gnpxxoqnd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gyvtmbslg.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gnxbjkaxp.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gvnhrufqv.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gmaxrilsa.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/gdnuswacj.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghgpbiehs.sHtML


<!-- 参考信息 -->