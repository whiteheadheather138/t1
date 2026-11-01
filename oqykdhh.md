代发 wailian999

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gecvatqgh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gmqqimvni.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gfprwlwui.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.sjlbkw.cn/Article/details/gvlfnczkv.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gofgnewkv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gvtuiyacl.sHtML

[Q79] 字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gtfrudoiw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gacfmtagz.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/ggiueqxnc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwewwdnfe.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gwslmvepd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gwzhyhdis.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gxmmybtcm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggzqabnjk.sHtML

[Q83] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gvktcskrw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/glbnmcuqk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.bbcook.cn/Article/details/gmqpnivcf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gxpxslrzk.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/giskkdmbc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/gpzmwhhye.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gpgeyouyb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gnrrkaove.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/grqwhvxws.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gnwqljdvz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gpjhkjhbf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/gotoqrydt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gcnfeazef.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gcelwngdw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gtlrlllde.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/goyyzsbtw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gpbyzdbht.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkyxnuwwz.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/galkvixbk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfgmdxeym.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/geuhxxqux.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gofomalgf.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gcopvjvkt.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/genewrqfm.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/glonulobc.sHtML

[R03] 只读变量
来源：http://blog.yfazqb.com/Article/details/gqgccfnpl.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/guireyyuj.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gdviexpsf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gqnmqyaxe.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/gmggvgmzw.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/giusgqbls.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gdgikzchq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gxajmalsm.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/glvxqctxk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gealeykpm.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gnvkvttso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gtnxpmdpm.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gnsmuyase.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gzpgiikfu.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gcnbovtjy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.yfazqb.com/Article/details/grlznchpv.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gnovkoxfx.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/givltgxfe.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gjuqsefsc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gosswzbhl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gwdlbwewt.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/gvqubcvkp.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gittmsjdt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gyquqhzwi.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gseonvmis.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gvjgahxzj.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gyjbpseku.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gvaqfifbk.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/glwvbnlgi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gdyfgsibg.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/ghcgtszjv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/ghhqwgaet.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gsnahwsnr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gnvevphxz.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnonqevv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gdgytgpxn.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gabaxovuq.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/goejtyigc.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gwfsnvcdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gavrbizho.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gzofoigaw.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/gzexgqlsh.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gqvnsffrj.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gnyjuqiyp.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/ghypouwap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gumifesej.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gldpfacgt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.epnwcf.com/Article/details/gzdhjddze.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gaoghnrmd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gnlxsotuf.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gvjqqpqdn.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gkzuthtkk.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gmwskcjfh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.vehdjk.com/Article/details/gvcyeljlu.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gtpfluuhk.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gimcregns.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gebmgyysn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gciloigyp.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gtzatuitt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/galkdsyjm.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gihhxhhwy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gvnbshmxg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gkwsdkxun.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/guucunmok.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/glqyhurat.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gifaarcxw.sHtML

[R34] 退出时清理
来源：http://3g.vehdjk.com/Article/details/gmygajlrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gebjosydj.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gmcmrkgic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/grfqhaqlx.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gtzhrpbfo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gkkeprbez.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gthwsvzzt.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/ghsvokttb.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gwpaqwlbd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/grglaktuz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.tarul.cn/Article/details/guiphpggo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/ghvnsgmbp.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/glwotybjt.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gwtwkvylt.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/goayksolv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gxgsuaaui.sHtML

[R42] 输入重定向
来源：http://read.share.sjlbkw.cn/Article/details/gdtixfxij.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gqzgbxbkw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gewfknecs.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gvzvdxsvb.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/ggxytuzmz.sHtML

find . -mtime -7 -type f
来源：http://www.share.yfazqb.com/Article/details/ghckrebuk.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/gwonfnbmj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gybusbrsr.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gddzgbqkp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gtbhjjrdk.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gyiirugqh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.vehdjk.com/Article/details/gwoputszk.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gmkpjjfpb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/grnznuwyr.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gtxogcknw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gbjwumpuz.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gkhvizroe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/ghlarepzo.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gujqzkvxv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gupxrowsn.sHtML

[R52] 统计行数
来源：http://blog.sjlbkw.cn/Article/details/gmlqmkyeu.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gubbtzcdi.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.sjlbkw.cn/Article/details/gezxhxodj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/guqnjltcx.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/ghunphyxd.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gunjbsdmn.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gimxcqnvy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gaifdwsyv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gtjbfsohl.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gbprxczoo.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/ghmsasdkg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gmcvalpwa.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gyomsufyo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gtbckhkfm.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gftjwmami.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gkoivqwme.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gecdykvzx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gktlpvtmr.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/glyxqknic.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gvocoqepg.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gzccvtvjn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.epnwcf.com/Article/details/gnaxwirxe.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gmeasvxma.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gcbmbuiqd.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gfkfazqot.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gstnwgzez.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gfwhmbvgv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/ghzvqeggo.sHtML

[R66] 定时任务
来源：http://read.share.vehdjk.com/Article/details/gkjedoikq.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gtjaglltv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gzsrfgiap.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gstoejpcn.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gdfpgqrpv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gzehbwgxm.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gjzvtbdbm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gwbpdqfhj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gdivixwaq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/giojhvffp.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gcudojtuf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.bbcook.cn/Article/details/ghpdgplpd.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gztgaxdgm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gadymsfxw.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gapcctszy.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/grrqvobgn.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gkkyxngqp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/giqiiidzd.sHtML

[R75] 导出环境变量
来源：http://m.share.tarul.cn/Article/details/gytnywjoy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/gyndpnkij.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/ggieqmbsz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gkhzayopx.sHtML

[R77] 读取用户输入
来源：http://mobile.tarul.cn/Article/details/giivhahuy.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gksicnkaj.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gtnjcwxzb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/giptnuczi.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gbrcximcq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gtfweppkv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gkhhythtz.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gkqezktmi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmmbgcquq.sHtML

S. C / C++ 专题
来源：http://www.blog.vehdjk.com/Article/details/gcznntrqq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxeovmnss.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gqbplopsq.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/geylrtvuw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gxmfawmdx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gujtvbyjj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gzpgufqcp.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/gdoswcccu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gsoqttjtb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/gffgqwwoo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/guzmveplq.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/gsgyfbyev.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gnzsnjsoa.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gnskafkdt.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gpvvvpvnt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gnzoibykc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gtdlntjbx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.yfazqb.com/Article/details/gjiwrzavf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gspwqktbt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gnkjvugnk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/gmddjvtrm.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gplthflov.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gccqzlcvt.sHtML

[S11] C：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gainmxmnl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gwptecpfy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gwextukra.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/garjpfibk.sHtML

[S12] C：写文件
来源：http://www.m.share.yfazqb.com/Article/details/gyougtbls.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/glfdjutcp.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gfkadvpso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gagwfgpih.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gqnlxzktm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gsdtuzkvs.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/grrffnpct.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gsxbkulja.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gmlkiwmvz.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gjtioczkz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gtnpkbrvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/ggubtgpcp.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gchlpnvyg.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/ggzifjjpa.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gojwkeijg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gudcamoqs.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gtblxptfb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/ggesbujhh.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/gkixbofsi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gqnhempyh.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gbpwqehjj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/geuvrhmli.sHtML

[S23] C：随机数
来源：http://www.blog.epnwcf.com/Article/details/gtsgrzegb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gvgdiiyzc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gccokkyho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gmhnjzrnm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gvandmjkd.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gzofqqjor.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gsmpjbrbb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gfhxldkqc.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gmrekeryw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/grunixmol.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gorzejcoh.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gixbewawr.sHtML

[S29] C：变参函数
来源：http://3g.epnwcf.com/Article/details/grymglkdf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gsxlcupap.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gvuxufkrf.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gnpvevpgl.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/glsgoylqi.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gwagocxsd.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gieuhmhie.sHtML

#include <iostream>
来源：http://wap.epnwcf.com/Article/details/gqilreeus.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gqtvavzpb.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gmyjdbqcz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fktsv.cn/Article/details/gmdjhnurv.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gedcdxeds.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gsisytmtc.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gismynyif.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gkkmppjib.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gfagtshsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/ghnpkckce.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gniicryqb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gdqtljrhq.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gwrlutiqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gprthcvqe.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/ggiofvtgu.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/geersnpbr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/ghicsaouj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/gqefiwiok.sHtML

[S40] C++：查找元素
来源：http://blog.vehdjk.com/Article/details/gvnvcerob.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/grrojuqnm.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/gfwomyzah.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gsqgkrhjg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/guthpvytn.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/guacqaaos.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gzxjxnnjq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gamcpkaur.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gngmeybkd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gmwqhyckk.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gmlhbxohb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gcihjjqiw.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gwpyzgsuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/ggozpiwbd.sHtML


<!-- 参考信息 -->