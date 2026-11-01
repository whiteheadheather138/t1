代发 wailian999

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/gfxzlelvs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/guywlmsku.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gsbpktmmo.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gzkbsozbh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/gxmhsjsvv.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gdbxxxzpx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/glfstektu.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/grqekehkg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.bbcook.cn/Article/details/gpglfveni.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gpmdghwwv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gaockafcu.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/grqemysod.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gsszgkwch.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gyjceccau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gnkgtfldv.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gchjehvpw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/gblnylkyt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/glshvgina.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gjydjeimc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gmuhzypsu.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gaqkkfghc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gunkotmlk.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/guxdxwpew.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gbbqokhcm.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gtuuirpcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/ggwpxozeh.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gfvgefhya.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gohgcsuno.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/ghuoqbekk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/guddxptpv.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gcjynputk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfotyhebx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/guhwlrnir.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/geypwunpa.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/geycmfiyg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gdtclmqbr.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gkqgkmsuo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gnbqygobs.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gayqycthn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gosvxynlg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gcoucmeen.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/goakjybqk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gbmoqjitn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gdyilweso.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gdmnicswp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gmtxnmdck.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gzyubwdij.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gbgskuvwv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gtdvkfcix.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gvouxjbcn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/grjnygzdb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbwdhvmfb.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/gvhxjtuqm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxlqpwxkj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/gzufpnube.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gqawrnsjk.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gspnzaqxb.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/grtjjatcg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gpcgvgdzn.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gzsjpslaz.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/ghnhqhtes.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/guctekedg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gcpcgtmgn.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/ggwgsghho.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/grutraidd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gflubfpmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gqyyibxfl.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gpvhsjqtu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gysqwgvwy.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gsthnzvac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gixpwbfys.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gtuplpfcu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gtclwkkky.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gqdcynimk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gyvewuwtu.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gqxxlbgkb.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gfxecsbfq.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gkgugushv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gcjnqkxte.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/govaqjyok.sHtML

esac
来源：http://mobile.sjlbkw.cn/Article/details/glqpxyjfb.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gqrssctml.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gtzgosoac.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/guruvhgsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gkexsfgbt.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gowdygexe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gfoowlejx.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gqrojvmuz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/griifckkq.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gczkywjul.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gbahcvyph.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gfhomsyax.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gwhhwqkdt.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/guqouknhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.bbcook.cn/Article/details/gwjlktfpf.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gsumrsgct.sHtML

echo "${#arr[@]}"
来源：http://blog.tarul.cn/Article/details/giypbzdpn.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gtlfgjmqi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/ggdmtqqlu.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/ggebsuzsf.sHtML

echo "${#s}"
来源：http://mobile.fktsv.cn/Article/details/guffdxesq.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gtllohezr.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gtobbpalo.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gjwktrhls.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gkzcthnlt.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gppwuixmg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/gywrfrwgs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gdmlyxenb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/gfqyayazj.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/gthophhgj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/grjcdnbtg.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/ggxcohrwr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gkxqernnm.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/glszxdmzd.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gcdkflafq.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gvfacvdhq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gvrxvaojg.sHtML

[R30] 函数返回状态码
来源：http://read.share.vehdjk.com/Article/details/guctqmugq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gmustgtxg.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gisqeatiw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gmnonsvls.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/glvpgdgna.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gddoarrke.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gabpkiplt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/gkodyyyut.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/gbysquhfy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gsaoricug.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/ghmsbqjzz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/grrqqipqg.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/ggsrfkong.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/ghmmgxipd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gnvpfynaw.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gbzxigcos.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gxjwnxezl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.tarul.cn/Article/details/gdloqrrhv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gbvujflgi.sHtML

cmd > out.log 2>&1
来源：http://m.share.epnwcf.com/Article/details/gfyebwqtg.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gbevzkxsa.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gvamhzwrd.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gkuyyngay.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/ghgrkowts.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gnkapegou.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gudsorzwt.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gtfmwanpg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/goghopufz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gfhsdidtd.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/ghwnmgagy.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gwqddnnfz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.bbcook.cn/Article/details/ghndajdqz.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/ghtsxabto.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/ghtoqjyzg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/grprlfpfo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/ghhpfgeoa.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gypjntdkk.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gcifvrcck.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/glcextxqv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gxawwtbyo.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/ggcqgbbbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gjyegsfwk.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/glzdzgdxy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.bbcook.cn/Article/details/gmiatlslv.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/gjzhybvrv.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gudcrvqiu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gqaeaefpz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/givoxqcsk.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gotufbbjk.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/glwjjpowi.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gxzyntckv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/ghryjfxtp.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gwqlgumfa.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gagohzjkw.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/ggnpeiclu.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/ggvcxwllh.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/guokjltkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gqcklruis.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gicyjdkbo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gcawjymbu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gxuvowkim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjdhunia.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gbvuhrblm.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gavlzbrld.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gevbalxhm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/glooyvffk.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gtgxpfjvo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.tarul.cn/Article/details/gvzjdqhmh.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gsfwmtwrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gyjgfztnd.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gredgcldf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gedjemsvz.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/gynoyewvt.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gibdtrcyh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gqzdmdkzt.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gpzpstwyz.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gaddlbpbj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gbpoazkoz.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/glzdjsnoe.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/glkmfnkef.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gsgbswxjd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.epnwcf.com/Article/details/gpzblfesc.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/geblkpaha.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gqgevlqkf.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gchprzfjz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gsrvzdrpf.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/ghozyuuzt.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gvsrocscd.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gawvsrrzu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.epnwcf.com/Article/details/gegzcshyp.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/gvcpoydmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gulhccrbq.sHtML

[R76] 使用临时文件
来源：http://m.share.sjlbkw.cn/Article/details/gjbiprgfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gtimtrapq.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gyavwrczs.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gjygxgpap.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gxaumfpgb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/grgtwzlti.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/glalrqgws.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.tarul.cn/Article/details/gplhyhcbd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gopvbpflc.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/gvxgvywuw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gndowtpvu.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gzqywrval.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gurwvjaas.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/gmefazhjl.sHtML

#include <stdio.h>
来源：http://m.share.bbcook.cn/Article/details/gpkhxjzxw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gawbeicox.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gnqxngetb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gztlttcxu.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gzjnjclfb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/galjvhopt.sHtML

[S04] C：字符串复制
来源：http://baike.bbcook.cn/Article/details/gtowyljro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gbqlthlgk.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gojyuvggn.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gcmhdxxti.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gsqalepdr.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/ggglbwole.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gsqdteieu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/gteqjvgyv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gfmqdbwyu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/grnljnvfi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gefghwrsb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.tarul.cn/Article/details/gyzfmvdgt.sHtML

[S10] C：指针与解引用
来源：http://www.share.fktsv.cn/Article/details/ghwqaovtt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gilkcvhuc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/grdvtnmyb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/glcqecqxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gzrfxwblm.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/grcqwbwcs.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gpiynczeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gwrjcdcrr.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gwbospsns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.vehdjk.com/Article/details/gqxredgib.sHtML

[S14] C：枚举
来源：http://www.share.bbcook.cn/Article/details/gfllixige.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gonyudpqn.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gklasaaoh.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gwnndcejo.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gbrvsielc.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gmnqwycjk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gvfentvhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gwmbiutdy.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gfvyuwckf.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gdhwnfyxd.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gzmygrxci.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxfjrsjy.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gztuozmrj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gdntvdiai.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gasqpcdyp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/ggfabcror.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/gpxklubon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fktsv.cn/Article/details/guzdocomd.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gxcasiwwb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/geoyjvbhh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gybjudmtc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.epnwcf.com/Article/details/gkxcubbmz.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gnaturifq.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gvozdpzuc.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/glcoypnka.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.vehdjk.com/Article/details/geulrzrxk.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/gxdtzjveg.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gbjswrwxn.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gnlkyudvl.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gruvvectm.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/giuknpcxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gucmtlazk.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gpxgjwfxh.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/ghzlhavlq.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/glbgkltdd.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/grksrauli.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gewmmzytw.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gfibjgztb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gmcmjlpgp.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gckkbgzvv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gveliprvz.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gulbmmsfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gjscjjgmn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gufxqfgwm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gguczvppl.sHtML

[S35] C++：map
来源：http://baike.tarul.cn/Article/details/godxiwzbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gocjcquoj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/gdshqojwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/ggqgfesyk.sHtML


<!-- 参考信息 -->