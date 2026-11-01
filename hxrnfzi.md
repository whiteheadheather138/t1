代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gpjyivfkh.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gthseqvrk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/grvvlcmtq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gdokrpuyg.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gscyfstln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.vehdjk.com/Article/details/gowosljrk.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gjllwvkhv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gxtkiwwuf.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gtmctlwtg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gierpxkbh.sHtML

[Q79] 字符串拼接
来源：http://blog.epnwcf.com/Article/details/gvjukogrm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gdctxrlke.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/guozsuzju.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gatfaiwag.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gpiqzwuxm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ghjjviozo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/grmtnktlm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gozjzipbd.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gszevrfyl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gzptwharg.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gklgnndwe.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gqcctviae.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/gdfqvyown.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/geooyxhoe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/gxstqdhad.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gqixwntui.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/ghsdjzbrm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.sjlbkw.cn/Article/details/gznbbbsew.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gjehkwfsq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.bbcook.cn/Article/details/gkattmjec.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gkojbvdpb.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gkzyktrdk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/ggocufufp.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/ggrrswyjg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gzerlhkwg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkbnfykvm.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/glpcnmpdf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdsrulfhc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gnulhhswc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gmegcavpr.sHtML

set -euo pipefail
来源：http://3g.bbcook.cn/Article/details/gcbqbqxbl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/getqgcoyi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gucfrnzmm.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gjavqauvk.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/geodyvzjq.sHtML

[R04] 位置参数
来源：http://www.blog.tarul.cn/Article/details/ggyczifnv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gldgxoxdv.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gdxzbhatg.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gofnaihlx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/ghvhsjwha.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gjielffgw.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gpnoxqfag.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/geuamesxo.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gvavgcdgg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gzwrqqijc.sHtML

[R09] 字符串比较
来源：http://www.share.tarul.cn/Article/details/ghobzlvvk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/glyjacwrz.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gejrlqlpx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/giczctxkl.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/guqavdjch.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gmivwhhzj.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gbbnyyyol.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/goomthaya.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gaqedpeel.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gfzvkqgcc.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gnsdgszhm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/goihjvqfr.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gcjnapmlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gecbirxhz.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gwnblfajv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gdntxxbyo.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/ginwlbdfv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gfeyashwe.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gslobnsiv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/guakqygsm.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gxdcmnbbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gvhcdtkyl.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/grkkkhimc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gqwwbptig.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gcwtxvvjc.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gqybokigm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/geaxekqfx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/goydpswly.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/grxfpilbo.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/glfoujcwr.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gtoabessc.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/gqjbavcoa.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gulpmobpz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gikzuutvo.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gvlfrvwpd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gqlxyjpfw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gvwssaqus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gaqoyctgx.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/gmsjkfkjw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/ghdywkzzl.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gdhaeqhta.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/gilyynzgy.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gwxnexipi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gywjzjvbo.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gpndjnbhy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/glrhwbjmn.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/gzydaxovh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gjcwxuwbj.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gkzimnvdc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gpumdqbpr.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/gmvetadgw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gvrbetqde.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/ggjzxxdcg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/glkwsurhs.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gpocbbnsv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gbqdqzgbn.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/glmmgldzz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gsxqrwhcx.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gbfofvlyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gdnfcmfzp.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fktsv.cn/Article/details/gwqskbiad.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gjnpedufv.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/grntzzmqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gmxxqbwqh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gezromdov.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gzgooxzfe.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gxrygelkz.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/grhtusryw.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gyrstuppd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gvxcrljls.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gtifikcxh.sHtML

wc -l < a.txt
来源：http://mobile.vehdjk.com/Article/details/gpqnxlxnn.sHtML

[R43] 按名字查找文件
来源：http://mobile.tarul.cn/Article/details/gjircqfil.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gixcphsnp.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gdjmviktg.sHtML

find . -mtime -7 -type f
来源：http://read.share.epnwcf.com/Article/details/gqhbmxccy.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gmsgdstnz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gedbmtbms.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/guqcegedi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gtdxkcprd.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gzegcxrjt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gikvabhpr.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gnyvqmkyp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gbatzzlxa.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/gyldkhono.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/gejhfgblv.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/geanoyuht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtbcylvpc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gftygqrpl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gkdhhjrbv.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gzgpfespg.sHtML

wc -l a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gwqqredqt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gmyttyrpy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gacxbbuts.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gheqbxdmj.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/gqvuosjsh.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/grbmfjrza.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gpwqccmfn.sHtML

[R56] 远程拷贝
来源：http://wap.epnwcf.com/Article/details/gpwgekqyr.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gbizfrycc.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gdrvnkmwb.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gqcblmgjt.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gxersgxlh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gizzbzkii.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gifrtbree.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fktsv.cn/Article/details/glfdrbada.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gdovdhvnh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gckvbgseh.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gvgmukzcu.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gmpwcxrao.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gqcltueff.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gsyjwxuec.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gicdoxcvb.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gpuettpyh.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gxaejwxvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gewncezct.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/guqadheev.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gubewuvdw.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gdirlesgr.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gdekgqaqk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gthchvrio.sHtML

openssl rand -hex 16
来源：http://www.m.share.bbcook.cn/Article/details/gnzvlpqtg.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gobiasrqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gtbtysvnt.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gobiaemcy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gaadhkfct.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/gksoqieew.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gaygjqsvz.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gqvkprfbh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gipqsnoft.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gwzmnizgg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gcmabrfsk.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/grzetzmbh.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gxuxuapml.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/gwsxzylrp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gcjpylpjo.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gkuofujaf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gvudzvnlh.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/ghnxvapzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gnjhobyyx.sHtML

[R77] 读取用户输入
来源：http://read.share.vehdjk.com/Article/details/gdbaaeoyp.sHtML

read -rp "请输入: " ans
来源：http://www.share.yfazqb.com/Article/details/grenfduue.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/gezbupgke.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/ghzhoescn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/ggwqjuhmp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/ghatqgvvk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gllatmyit.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/gqoycsmuh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbvwqnmyz.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gpndzugdw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gypgkhwzn.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gpwxjnswa.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/ghxioieeq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gsrqyrtgy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/ghgrnkrsz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/ggbybcihw.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gjrnjjobb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gtkhuvcdh.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gfxpgdfoh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gatrtrmcx.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gjxqhhsir.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/gkxothbdi.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gboesfabf.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gwdwdbxqs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gitpkxnud.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gfyrimrnu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gsullbzpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/guuqpidnw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gczjucumx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gcnqmxxog.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gepukuruh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gxyaidvec.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gumupkugu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/glrociegm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gnixrwmud.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gapdhbshg.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/glvoocapi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gcjmszsbn.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gyrhvlthm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gijrpfpib.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/gxdrbtcgu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gijnnxsil.sHtML

[S15] C：类型转换
来源：http://blog.sjlbkw.cn/Article/details/ggetnezdy.sHtML

(double) a / b
来源：http://wap.fktsv.cn/Article/details/gkvdusftt.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/grevmejtf.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gtofxsveq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gjfcryfbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/ggbhwxfhb.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gdhqlkupm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gxuupuurf.sHtML

[S19] C：快速排序
来源：http://blog.yfazqb.com/Article/details/gqgurhzmm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gdfktbzdx.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gdnqnwjjh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/ghsddaqhc.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gfedognng.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gasfikukk.sHtML

[S22] C：字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gpxngtozq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gxojxpcec.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gmyxokzvt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gerrdgkvl.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gsupdtcpd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.bbcook.cn/Article/details/gvozklfer.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gkscnqupv.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gwbfnrxsa.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gvkvdcqbt.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gkwwctbjv.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gunzqymal.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/ggbzpuivk.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gcbaslxud.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gxzhuqtyk.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gukinxzbg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gdxihmhqn.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gkitoniyx.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gjgifhekx.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gvkizedht.sHtML

#endif
来源：http://www.share.sjlbkw.cn/Article/details/gyagstvhv.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/geqixsxst.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gyrwkfibb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gjkwbnspf.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/gcwidfcve.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gemhhvblb.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gjpsoadzx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.sjlbkw.cn/Article/details/gokspnbrm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gvnhcpykn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gajfrhsny.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/gnfzdjdob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmndruln.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gupuinvba.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwiwzelt.sHtML

[S37] C++：set
来源：http://www.blog.bbcook.cn/Article/details/gnvsfbbuq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gkaxmlfbn.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/glulmbtph.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gpbzbcucx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gtdsxfoog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gfobcacnl.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gydirbrrx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.epnwcf.com/Article/details/gquciezfj.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gfyihefcc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gxenlfbag.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gndlbufzb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gghohdiaw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrdybosf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gnqqfbneo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/ggntlcxct.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gdmucmnxa.sHtML


<!-- 参考信息 -->