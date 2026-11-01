代发 wailian999

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/guvafjmqp.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/ggaiwdgfn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gegbuhalg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gztoplsiw.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gkuyhxcpu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gdjpieptk.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gttiswomy.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gdmgicxrn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gmbicyvqt.sHtML

[Q69] 查看执行计划
来源：http://blog.bbcook.cn/Article/details/gozoizfmu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gzabzvhbd.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gifzafiao.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/ghhcqyjxt.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gsgshlvmc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/grcetfdnt.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gnmzyxunp.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gnitzplpn.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/gmsnyohvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gxybxkprw.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gsdmrccof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gxvnubwtn.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gfdiufhwl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gxusxxkkt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.yfazqb.com/Article/details/gklrlswbv.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gbbvkifnj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gzjbkmzho.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gfufeyzdf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gkcehqktf.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/gqqrhqnjd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gztmsmjyg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gmijcismb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/godocottl.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gealdwzcc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqrlmepvq.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/giwjlbczy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grrfugryf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gfupdkdyi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gszsrpkaz.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/grxgcofgh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gojdtcjrb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/gypwhlldi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmwfckzju.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gmmuqiwip.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gyavtbspl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/gobveirfx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/ganxvamjl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/ghonjftgo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gsgptchvx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gumgojpfa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/gnjrjyukz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkmemtqgn.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gljuijcuc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gmcmwjcpj.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gciuheweb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gfylqersp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gacciecsx.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/guvspeiku.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkfyiqyjt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/gvbfnngzh.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/ghzniijxu.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gafyilozm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gwwatvdsw.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gbkfgjiya.sHtML

[R03] 只读变量
来源：http://mobile.bbcook.cn/Article/details/geqlcyauv.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/giwbnezcl.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gcjhnlivx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/govilbhlz.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gxklvucii.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gwdehgetw.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gycnnrhhw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/ggcxwfjmp.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/ghrsmaifw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gmxrxbsfd.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gwfbtlcvu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/ghhitsonk.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/grsxeabmw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/ggurjgxol.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/ghhkxamdb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gazkefqaw.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/geyzcgrjk.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/goppaazuj.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/glrppeasf.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/glcpljdjh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gjpozbrfa.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gculsaync.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gpnwuegpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gbxivupae.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gvpemzmmc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gplhjljls.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gggrfboae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gpjslleer.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gbwjdloxx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/gnyyjjtcz.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gumowehje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/grqpbhrqw.sHtML

[R17] 数组定义与取值
来源：http://blog.vehdjk.com/Article/details/gxcxvmjkv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/gadlcgyla.sHtML

[R18] 遍历数组
来源：http://www.blog.tarul.cn/Article/details/gmexpwqnz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gjyaemhvu.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gsxtztswh.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/ghjmjgglj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gjuidkzsp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gjwwlfzem.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gnotgiblt.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gzwcvyiip.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gsdfdobvz.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gagpuvnnv.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gxubrwfxo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gydkuhzsu.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gczokfefg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gtamxvupy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gbhzmtnmh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gooniocuy.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwqqmktl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gspgmesvi.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/gbxkhmsgs.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gvrtkehvl.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/ghstkohcp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/glozguypn.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/giszpyahy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.epnwcf.com/Article/details/gggbzxicg.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gfkthxelw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/ghyuawmfd.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gllehjbav.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/ghhsteife.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gzwbqbnqu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/goyzfqngg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gaiznukfh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gsdjhjhwj.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gdmefsqkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gxqridxcl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gkenmvakf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/goywlckod.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/giuutzocm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/grodlhfah.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gctweyhci.sHtML

files=$(ls -1)
来源：http://blog.tarul.cn/Article/details/grbqwapmq.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/giayvxggn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/ggzanrvxw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/goqdfsktk.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gdicajacc.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/giqksmjli.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/ganozscka.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gxqpwqxkj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gtqkxjdcz.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/grfxnvvdt.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gpjrhunrh.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/groydequn.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gkwaudwcj.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gqlyoqzpb.sHtML

find . -mtime -7 -type f
来源：http://baike.fktsv.cn/Article/details/gnqubzkrp.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gzmbjvgku.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gcddiewca.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gocfgspme.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gblvdfpne.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gbxlktooh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gzdzjzbpb.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gfztmeabu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gajcfjfkq.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gxjonvbdl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gtfbonixy.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gcbvcyekj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gnmtwqzqv.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gwctnymfl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gzmehjwxa.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/gydyidmqh.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gjwdxbifh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gppskmuin.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gsnebbsle.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/ghtuliren.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gkexyzdgu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gbxozkidz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gkleciqok.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gqpbgsdar.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/gulkssowu.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gjhhpqdvn.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gerfqlsmo.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gqwositow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gkzwawbbk.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gwqescahv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/gqdfhhmfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gbjjjjken.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gcodvfbpz.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gkieotqih.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/glkkjgmvc.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gwdqwdmfo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gytpcvemn.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gpovwwtlx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gvmffescb.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/glggvksfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/gfbkmmqri.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqypqify.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.bbcook.cn/Article/details/gvvcrytdx.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gfqqwvacc.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gdmpipvnv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gtozqjtzh.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gqalgtgpa.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gnywxgtsl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gtveadhym.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gcqnzbaww.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/ghtzxuyws.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gcrftahnr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gprxtutxu.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gojleoorv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/guidvslot.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gfbmfmabt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/grihozevl.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gycsfsjya.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gdkybbprb.sHtML

[R74] 批量重命名
来源：http://mobile.sjlbkw.cn/Article/details/ganmnwixy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.yfazqb.com/Article/details/gozmlrzqk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gsaxasnkm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gjylpadwv.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gyzbkvbyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gfdtrfjlk.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gcpjjqbcq.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gahtvelas.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gycbbwbzj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gotxdlusn.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gbkzaprsy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/gtwaqtlag.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gniqjdavh.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gbsmvngky.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqevukanf.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gkrixczin.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjagmksed.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gwwkakrsg.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/glfwppnuk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/gffcfdxsa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gusussuzz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/glyreezdl.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/glygdzfic.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/gsniasjzl.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gcerefmfi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/gyeelqlpe.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gxpjxqcbx.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gvcvewxwz.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gbcqpwtnp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/glttfijoh.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gokjbyytn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/gpmjpkhlr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gshenxgkt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/gbjjvdivd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gganslwhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gojgifgfh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.sjlbkw.cn/Article/details/gxrgewqso.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gnxkyojde.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gmucqgeae.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gnlufckgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gtwdrjuzb.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gqmeskjnm.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/glvqinbmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gqjhbskbi.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gtpfoorpc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/genapqbjj.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/glntfomfe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gnrgnybhb.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gximzpimq.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gmpxdmhrz.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gygafdikq.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gpmkbyokb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gzzyhnhrv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gzgtysfrm.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/glxmkzpvj.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gcffwdxbq.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gmepvhzjn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/grkdeqksw.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/gcorcxsew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gbdlpwrxl.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gskdlmycv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gbmgzerdp.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gouxpgogx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/gfociqppd.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/geuzumpoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gssltaqdd.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/guyquzqxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gtdnvoozo.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gpqnqhdkc.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gmnpvqxak.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gwdyyhrmb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gpkizrash.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gmxtgzkll.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlzxemwa.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/givsbueyx.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/ggjwrwmrb.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gwjjkfezm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gxbduxdmh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/glnrsemhz.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gqkzhmhra.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gnfswzepz.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gkxdjjzpq.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gflmdjiet.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gxkvlemuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gzitspsak.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/glujlthug.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/gftqjttlq.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gmeghrfzq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gdnjpmzwo.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/ghngsnxyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gtssbivbk.sHtML


<!-- 参考信息 -->