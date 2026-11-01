代发 wailian999

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/gwjngrzfa.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/getizqehp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.tarul.cn/Article/details/gsannnzsy.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gycqlhmno.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/ghdgaiift.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gopybvikg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/grybijyhn.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gzwdvzdqe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/geapowsss.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gpqgtqbqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.yfazqb.com/Article/details/gijtckogf.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gvlpypwzi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gynxqirwe.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gckdcjypc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gkkizoxjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fktsv.cn/Article/details/ggvonkdel.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/glkdphdiv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gerdwdyha.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gwoqhyzmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gihtgtfgr.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gfgomcnoz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gequgpmkj.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gsxwdcztz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gcgofopze.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gfuhusyrt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/gcxmstwwv.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gpfsqsmcv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/giiozogcy.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/giojxurfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gffctazhr.sHtML

[Q83] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gjkwedbfu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gxulbdzme.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gslxgkcca.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gjvyiqfxi.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gseditkud.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/grvtyxclo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gjpnjltlm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gpkfuubeu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gmzpzearl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gzpubzgtl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.yfazqb.com/Article/details/grzmizrif.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gofdwfkil.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gyturcsvl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gyhmzhitv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gspdloxqj.sHtML

[Q90] 生成序号列
来源：http://baike.yfazqb.com/Article/details/gqtfhllgh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gdztmepkz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqrtowlby.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/govjieosp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwlheidjj.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gqlvymngf.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/ghqhwdhzo.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gecrlhvjx.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gudksnavq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/ggrroeinq.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/grdrtnumn.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gitaiecag.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/gxljvkpyc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gxdibpxzu.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gtwukibfx.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gmndfsjcm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gxudzahwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gmrfwgtvv.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/goooteoeo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gulmrjktn.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gwiwwexjz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkadzeynq.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gytygapqb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gvdfjnajf.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gnyrdgosd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/ghknwqynf.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/gooqmvpwn.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/ggwuzuqsf.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/ghmdjqitq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gyjxtlmxz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/greuhkuul.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gcucykkis.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gnjbkwunw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/glluibqqv.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gmxcysrce.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/ggdlzvbug.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/geyrhdeqc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoekzvhv.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gkynyplwy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/geuchwafe.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/gmcojuhmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gaqvbskxe.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gxhtnxdbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gnpckrekf.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/grhkgpzwr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gpufaqsed.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gibrmeydr.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gvwsafbsi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gnojqprtb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gfnlnkday.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gnrtolvnm.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gxksznfvw.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gwrubetxo.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gbyfyffoj.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gyoommgix.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gexbozzyq.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/girlwynmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gtasqkakj.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gwuvnzgiy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gzppioakr.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gzqswqmsp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gwpnmyqhi.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gvsvaaasc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/gtgemmqxa.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gxzgoaduc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/gkgvjookx.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/garipslmk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gcyzguzsg.sHtML

[R30] 函数返回状态码
来源：http://mobile.epnwcf.com/Article/details/ggerfmduc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gsmhavwic.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gjhgygepo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gfbejgclz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.epnwcf.com/Article/details/gdlflwboh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gxdnmgxsm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gggogfkhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gsbnjntfc.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/gnxbhxtfe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gfkntxvkj.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/galcmlswe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.vehdjk.com/Article/details/gycokziqm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gcrpckvtl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/gdjzqozqk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gmmqbmkdd.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gyakoivov.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gttlebjaq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gfkkbcvex.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/gztasoimf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gltkqjyyo.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gqdikdtui.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/gucekutyd.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gbatkamem.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/guoankyfl.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gakwknwbv.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gjwjhdelx.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gzhjwxfry.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gpjfatbdm.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gzqrlxwbx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gxbaxkakk.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gwpxxigmv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gdzjtvtpn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gscktwubr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/ghroxisvq.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gmjszhktc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmpgwlyzr.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gkrgulxwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gbvtbklty.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gotrxozqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gcypzmwlk.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/grvqjmrsp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gebntphkg.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/glsitsbfg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.tarul.cn/Article/details/gkbaupxdq.sHtML

[R52] 统计行数
来源：http://mobile.fktsv.cn/Article/details/gioasxubs.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/ggbtlbtej.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gxgjrsewt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gdsvyzrff.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gnapvsvri.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gvcrrbump.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gnutkwjuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gkchmimoa.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gulvvnwgp.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gsbmebmwk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/glsxcdhsx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/gsxkxbwap.sHtML

[R58] 下载文件
来源：http://wap.fktsv.cn/Article/details/gzahaajzi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gfofgheby.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gntnwwntc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gjkymexqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gjdagyglf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/ghlnqedoz.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/geefyfyen.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gdyimzxzv.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gngovnggk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gwjxzzzvi.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gpqiqtmdi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gtnxduqxz.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gupniejfb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gzpciikng.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gwneljsnm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gnpjxpiwb.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gkedygscc.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gjwqrygzv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gvbrqjoyy.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gbgvycsyw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/giklqjift.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gainnznrp.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gvanmrhim.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/ghkzrbrho.sHtML

[R70] 时间戳与互转
来源：http://mobile.fktsv.cn/Article/details/gpkqrgyjj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gablveiib.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gqlfdvuii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gddqspzwe.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gybpmdmwr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gohueprpt.sHtML

[R73] 分割大日志
来源：http://wap.bbcook.cn/Article/details/gnmyuhkog.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/grmmohaae.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/gbzlmwpux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gsetwxwjz.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gcvrdpzjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/guebdheqi.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gwtksutni.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gknadobyh.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gomttbbtz.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gsdnwpldj.sHtML

[R78] 交互式菜单
来源：http://mobile.yfazqb.com/Article/details/gqpocoaad.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gbdmvclly.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gbtxxpbhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gwkyqfucz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gvakywmqb.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gkttpabfi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkvxwbvyl.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/gmtvbalxk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmbtrxztq.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/ggjyzqawt.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gznxznyhk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/gifljypdq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gxncuuuqk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fktsv.cn/Article/details/guywfdluj.sHtML

[S03] C：读入整数
来源：http://mobile.tarul.cn/Article/details/gxxvqhawy.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gtogglzeo.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gxdnubhzk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gzkozfpcs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gifynyxuc.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gctmnkzlg.sHtML

[S06] C：字符串比较
来源：http://3g.yfazqb.com/Article/details/gkilfmjlm.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gytuoxkwb.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gsojhrqqj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.yfazqb.com/Article/details/gjtkhevav.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.yfazqb.com/Article/details/gsltfzbzm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/goanoqplq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.tarul.cn/Article/details/ghvpsusnr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gagbmkbrr.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gtbugusyg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fktsv.cn/Article/details/ghwsqkxbm.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gdjogewmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gfkrmpuzm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gimviffmj.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gmroynlwt.sHtML

[S12] C：写文件
来源：http://www.share.epnwcf.com/Article/details/ghezuusjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gdyjzdyji.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gmwqenwye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gnpjoddco.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gbykbxkef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gojpifgds.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gpiuqbrpa.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/giumxtjqi.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/gszgvixul.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gwdpmojzi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gaubdmcqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.vehdjk.com/Article/details/gjxmxqvxf.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gfwlmnijv.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gdmyvxbff.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gphuldjdw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/guqqanica.sHtML

[S20] C：二分查找
来源：http://3g.bbcook.cn/Article/details/gbybnjadl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gvtmsprxd.sHtML

[S21] C：字符类别判断
来源：http://m.share.tarul.cn/Article/details/gdejkxohg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gsylgogqw.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gjejrolex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gdjdrllgv.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gcwpwpjok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gmraoayqe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gfhylkcye.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/glskgnile.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gsqjqlmen.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gvemrvnnr.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gdfqbdisx.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.sjlbkw.cn/Article/details/gflzvuwhu.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/glxgzxzmm.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gpfronovs.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gneajnake.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gbnehmhuc.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/ghworbraq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gpasoeeyv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/glbrfacye.sHtML

#ifndef X_H
来源：http://3g.tarul.cn/Article/details/grwmpkxqx.sHtML

#define X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/glyjvenaz.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gsijhqoic.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/ggllhboka.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gmyqqixlm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gyspemapr.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gqhskbgil.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/geokpjbxe.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gpmicaybw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.bbcook.cn/Article/details/goudvurns.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/gvywobhih.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/gbrjkkamh.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gyjvslvnw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gtfjncixx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/gjuhtdicb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.tarul.cn/Article/details/gjzdthcfa.sHtML

[S37] C++：set
来源：http://mobile.vehdjk.com/Article/details/gsvwcddpy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.epnwcf.com/Article/details/gfuolguke.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gdedbqlmm.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gruawdmdi.sHtML


<!-- 参考信息 -->