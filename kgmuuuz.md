代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/glgcrieyj.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gzbttgxuo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gqxqjesam.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/ggcxprihc.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gbujhmgua.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/ghsxksugn.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gggjdowax.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gqnwwzvkx.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/ggtgaryqe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/ghdgkylcd.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gkjqkaxkr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fktsv.cn/Article/details/gcpwfirie.sHtML

[Q80] 字符串截取
来源：http://read.share.fktsv.cn/Article/details/gewnhdxia.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwnaumtde.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/grujizshs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gftrajxdf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gyvgzijqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/guvzrohjd.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gyvocwasa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwiapenpe.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gefexhjsx.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gybpymjai.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gocbyljvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/gsvyyzdpo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/grsxiyswi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gjsnmodne.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/geozyplfe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gpthqrwpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gizdhmyra.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gpweiwims.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/godznquen.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gzvcmlsjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/ghwgxyojq.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/ghxyjznuj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gpjvhonfy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guqwtxnlh.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gmxbujxlb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbaqwtdtr.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gxuknvujv.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/grzyiofae.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gbcyyduop.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/guqefwzjy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gbcpzezza.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/glcqioqzv.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gxzfnweis.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/gcidvufos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gzcbcxhwk.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gncmiuozl.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/gaosarsck.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gitdassuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gswluptzs.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gemileoqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/gmionklmp.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/glhtibjzo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gxtcdkguc.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gkbtihurn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gabxpxrhl.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/gvoajtpme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gmbjyakan.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gbeskdyyw.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gdnnlgwcg.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gmheauzhj.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gekxybhnl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/golnethvn.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/gwgbjclhi.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gqkkjnnkc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gmgrmufpk.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/getorxswn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gethtbjxa.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/ggjvlybxz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gcfbywone.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gvahhdhsh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/galchtnwz.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/glsxwgzor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gyzqbdurl.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/grmnyjcgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gkyphqogt.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gdfocvnsa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gidugwhrw.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gkkvsdpkl.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gkitmsptt.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gwpogtwyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gkanetrqv.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gftusswrv.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gfxnbgxzq.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/guayfvkip.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/gtyflhxrl.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gbachngwc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gkutojhvy.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gbklfafuy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gsjtrzmcx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gsrbycali.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gubkuxyuq.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gwqrsrtea.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gvvtmgwwg.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gtmmzjaos.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/ghanbjdqn.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gcheuemvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gooyuwvgu.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gonjfgcvg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gebwegcck.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gzxqvjzde.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/giohpdajn.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gmrkqdshr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/ggebkycqb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/geqvaqgjh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/geaawzqep.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gktfvylbq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gklxthzzg.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/grlsctkgw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gfrheqlbq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gymivliwi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaxszesc.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gxpdobedg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/grblhpyyi.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gshpgwkjd.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gkkulzrts.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gdihvvysv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gtdffnavr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.sjlbkw.cn/Article/details/gdbdzyppa.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gplggpktb.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gelfwpbyr.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gujfhqkal.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gsrxdwfnr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gcmbddryd.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/glfrozdvm.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gttkqtget.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gzvnmslea.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gzqdwxmfy.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gtwkmohpb.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gxcmskjix.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/grrorsgff.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gcysxjxgw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/ghahrzqzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gjgvhpwxz.sHtML

[R47] sed 单行替换
来源：http://www.share.tarul.cn/Article/details/gotouupcj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gfgszojfn.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gmgszrcyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/glpuomwua.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gjgdalzka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/glanauofx.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gldmefbnm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gmhkciuco.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gntdtvmwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/giljqpyny.sHtML

[R52] 统计行数
来源：http://3g.bbcook.cn/Article/details/gpaznrjuh.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/guoqoengt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/ghkllnavj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gbjbitbfo.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gywgshgqy.sHtML

diff a.txt b.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gaijvpskj.sHtML

[R55] 压缩与解压
来源：http://mobile.tarul.cn/Article/details/gebvmeffu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gdubueonx.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/ghgwmzsrz.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gvoimpdev.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/gkjgtdytj.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gykbyhnwd.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gggfdhcio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gspbwwxzy.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gssbureyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/ghempnxto.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gseafyfwe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/geplmzufa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gstxfahox.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gdvhvtumu.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/golxcaohv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fktsv.cn/Article/details/gnfigoqio.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gjquaygoz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gyqiplwwj.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/ghqehqwnn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gzixxtpqk.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gmkunlmbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/ghfygknby.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/geashbvxb.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gnxmmrkzm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gwnymccjd.sHtML

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gshgobvqe.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gpnrldtye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/glwcadhix.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/geixpanap.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gxbwsheqo.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gzconwlsf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gsoreepmw.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gkherurvp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/gxmmnxsxz.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gundcfdym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gfalwewuc.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gjqutudmw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gsaucftlp.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/geegnwwom.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/glovrvxbz.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/gzicwqeeg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gyoilsodb.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gqknronxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/glxbxauif.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/gmbfifhoy.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gdfplazoq.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/ghgucoogw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/getekqovu.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gkyhqeonf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gtioroqlb.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gdxdtywdi.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gpehzunje.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsgxdigbm.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gcpdnyaih.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gejsdmkew.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gquzsdjhw.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/glztwfnrt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/gryakgosn.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/guszjgogz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/grjfjxcph.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gcwyhbyxy.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gcwikydjg.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gxfwvkwoj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/givaqqfkl.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/garjtznkt.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/gdrmtapui.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/galkpkhso.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/grhfkgjbg.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gmyyexdbf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gazfkywwd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gezmsgxto.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/guubgcnhl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/givjphanr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/gvqndreai.sHtML

[S10] C：指针与解引用
来源：http://read.share.vehdjk.com/Article/details/ghsvqhqzd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/ggdupvimc.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gkofuetpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/gsicylziw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gyzfhuwng.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/ghuwnutpq.sHtML

[S12] C：写文件
来源：http://wap.vehdjk.com/Article/details/guevaswvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxgqnzqn.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/goanwcyjh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gsrgdvmmp.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gnravkvja.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gapescvxs.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gssoaayhg.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gmxxvwoxe.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gfynedtuv.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/ggnbdtqcs.sHtML

[S17] C：安全拼接字符串
来源：http://wap.yfazqb.com/Article/details/gccscizub.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gurdjqujj.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gaynikhii.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/ggekqloju.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/ggillfbon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gbmpfszap.sHtML

[S20] C：二分查找
来源：http://3g.epnwcf.com/Article/details/gnzlgmhvp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gvlsaspcb.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/ghgnaneie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/ghaklmpit.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gvbtnkcgc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gtjautqhe.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/glmgatept.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gtamyjvsr.sHtML

[S24] C：获取本地时间
来源：http://wap.tarul.cn/Article/details/gbitiopmr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gheturxvx.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gsheehgnl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gulxbjkty.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gybcgwjvf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gagrcxxnh.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gljnvsaxd.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gtpoqfzhp.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gynopfdzy.sHtML

static int counter = 0;
来源：http://www.share.tarul.cn/Article/details/gwgstwuyd.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/gilqerqde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gaqdgkljt.sHtML

[S30] C：头文件保护
来源：http://read.share.fktsv.cn/Article/details/gxwwamsts.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gfcsnejif.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gorgwdjbv.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/givghokch.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ghrbhskxd.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/ggiisytpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqfkwqteh.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/grngflmxs.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/grbdpsmbw.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gxdbrxlla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gvqmzycjc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gjnosugsl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/grcezjljv.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gjqkuquex.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gmfkrhebs.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gtyhsogdh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gshkraqds.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gwkxmtgwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/guabdxlvw.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/ghwzwvpsr.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gzpyqmxxv.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gumaejkov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gkgvfzyky.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gcfdpmrdp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/grswvieyb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gbwfwymda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gxrvwionm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/ggwuweubi.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fktsv.cn/Article/details/gwspgkhei.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gcsmxzcce.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgbnghzq.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gtphlcfwn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/grybwjogg.sHtML


<!-- 参考信息 -->