代发 wailian999

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/gnllfzjsc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/gcogfqagr.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gsfyyeqbg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gzjvzahci.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/ghpncfkuh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gtdhmjjnn.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/grpwfajgb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gkxyvxtlm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gtaaozjde.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gnlymnhwr.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/glmmbuotq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gdntsigoz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gefewoubk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gjeeochsz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/gdjcjboiq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gfozthkdl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gopypunxb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gfyucsskp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gpnrgdhgz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhcvtqag.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gvqlfyqvs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gjblkuhty.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gxseapnhc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdxjulszo.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/gkgncozzw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvistukzc.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/ghdjgelad.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gytwoylae.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gfzptryys.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gkfxqziyt.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gjcwioagt.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gjqrscifh.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gawbmfuey.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/gaiabbatt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gtunsguvl.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gmcgwcico.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gfrwmkxiu.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gmwnpzbal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gcwgmlsbn.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/givijkkad.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/guixlwvpx.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gaavktrtc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/grdxtttvv.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gxzejamnn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/goluofuaw.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/grigxlzoh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gbqvrjeqx.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gfoprdbql.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gnqbqfuiv.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gjtfhscnn.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/grgsjkqfv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gkamzrtir.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gkvcgzfgt.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gyislyquz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/ggarlekpx.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gehjwcvvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gbvtphwxm.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gbcpogjoq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gnarrseul.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/goygykdwd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/gkxnrlsbw.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gvhyvdmkj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/grhhoqvws.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/geqorstml.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gnhevzvcl.sHtML

[R18] 遍历数组
来源：http://m.share.sjlbkw.cn/Article/details/gxdmeqvhn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/ghhdxkqni.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gpiwontig.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/giwdbscyz.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gcshyphct.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/gkhjervxw.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/glpmnbfgk.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gptovfxdw.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/grzcwwhei.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gwcadrtnj.sHtML

[R23] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gkjjhjafx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gcswycikn.sHtML

[R24] 大小写转换
来源：http://3g.tarul.cn/Article/details/gwjacxazc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/grphjovmf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/gmmnksvxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gcgoipejh.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gooirhtvm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/ggrxukmgj.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpagciim.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.tarul.cn/Article/details/gqmztidhv.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gennxvusl.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gbrfqwuho.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/guvmuyvsb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/glvcrenfn.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/gtxcvalas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gogvjytmt.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gthggsnuw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gcophwbpa.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/glnjzvuwn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gunsyenkd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.yfazqb.com/Article/details/ggrcjtjnu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gzxabvbhe.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gqxvitiay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/geppgzdrs.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gyhyoauwf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gxhiftetn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gvelwzgnt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gzqucxuzq.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gnccriuwr.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gqpvudkzu.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/geyuqwrsl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/grybmpios.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/gttdlisaw.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gqfkculps.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gwwrwyddt.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gmyndbhgt.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gwabiitxv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/ggvhixrfa.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gbaulrznf.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/ggbzftpgn.sHtML

[R43] 按名字查找文件
来源：http://baike.sjlbkw.cn/Article/details/ggbvclrtc.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gaphlkkni.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gpcyfeosc.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gpwqlqkyu.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gtyjmzhqc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gcomtpqsi.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.vehdjk.com/Article/details/goywcxcvh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gqwfipvkh.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gbovrmlqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gbdgrqqbe.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gipcbkgjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gsjsmydii.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gngeubnfr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/grnldfseo.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gujhdegqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/glubuimxe.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gacdjtqir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gdoijqqdg.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gedlfhyle.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gsrpxrjlp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gvrwfbver.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gifxyqasg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/gintixbpn.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gjlhbyvjc.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gxxoiljcj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gzpvztrww.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gtohfaprs.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gthbprmta.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gayqfzmbm.sHtML

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gqzcczdio.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gtjiltgep.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gochocwrh.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gpnwqmexf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gsouoaxri.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/glngedkhj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/gljyrulkv.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gxeegihld.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gdrpumjkc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.bbcook.cn/Article/details/gwgoqxcwb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqzbvqti.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/gpfvegvje.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gzfwdcldp.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/ggkbslueh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gktxomhlq.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/gwpazbowd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/grmvioyso.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gizfckkkx.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/guopvwivo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gpbbfstyp.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gpbycfyeh.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gtmympfax.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gubzdpvwd.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gfbolkoyd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gnmvymgot.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/giiuxiahk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gnvmbdurk.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gxrbtewjn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gfthfxvnv.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/gowbnzwmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gkkvqvhks.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gfklfljsc.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gwotjoiey.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gfklbrglw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gqxjpoxeq.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/ggbvmocsh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/ghyllsjvx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gbwrtshbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gdauglhex.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gkulrttza.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gnoauaadv.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/grznihmfg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.epnwcf.com/Article/details/gprwjafae.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/gdzxmvfev.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gwgfmsjeq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/gxspehuwx.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gbiohjpwz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwqorlktp.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gapojwtse.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gacgatuhj.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gdnfmbutt.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gkiyzpddt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/glfgveofr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gxyvpitax.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gpejeikox.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gjracagir.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/grphqckgx.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gljhyfahe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gpnaaqqoe.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gobzyxgnd.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gyfumrcgt.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gotxumbpz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcnaenri.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.yfazqb.com/Article/details/gtohbxmvf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/gecmhnpyr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gpcwkejia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.bbcook.cn/Article/details/gjidxtxus.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/ggtkesiir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/gyaocgecm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gpasrvrvg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/glvohlcwy.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gwnhlpaes.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/guvjllmod.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gphzekcgw.sHtML

fclose(f);
来源：http://www.share.bbcook.cn/Article/details/ghwamuegx.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkrtjxfdl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gwlgtwnjl.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gvzfjghmx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/guqaruvog.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gnxokaonw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gmvsrntkd.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gcsedyieo.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gfhnwexeu.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gsnuneohv.sHtML

x |= (1 << 3);
来源：http://blog.fktsv.cn/Article/details/gcxtzjgyb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/guvdoiljt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.bbcook.cn/Article/details/gdmbkptka.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxnerwmn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gmfylgupc.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gvpdcqnfs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gpxtsrfms.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gmvxghhgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gznaqmvuz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gbkpcazdo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gvdyvxvwh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/grrqbicpx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gzzutnnvp.sHtML

[S23] C：随机数
来源：http://www.m.share.fktsv.cn/Article/details/gmthzjets.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gzoffjlyo.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/ghvtqzbca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/gkndcsnxe.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/ghpcisdkf.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/geimwberg.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gyotlihai.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gxbgmdpjg.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gwgcmbyah.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gvgippvnf.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/ggdtenkjm.sHtML

static int counter = 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvntycsf.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/goiuqdide.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gpdhagrjc.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gfpxaorlh.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/genniyojo.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gbfqloawe.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gzcfvehue.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gfwekvqfc.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/gzgknasvm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/grkvcjixi.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gzfpxtmvm.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gkejcbcdh.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gulnxkqig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gqvlribxb.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gubdrrpax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gecqdmnvb.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/ghdqjvllm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gdmlzsysn.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gwusejdpu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gigmvhrxw.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gokgxsfot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/glynjniny.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gomjvpvbq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gntstyxqj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.tarul.cn/Article/details/gxahrvbcv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gduuxdhmw.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gcbwsfibs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gshixduhp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gkjtmyhrv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gpdcywzpw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gzprfeaqr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gchnfzmoe.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gzcyzmzbd.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gkcnlkxjr.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gjpjuxbzj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gzgubblkw.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/grzgszabq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/grgteljby.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gqmcorgkr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gabnnjmap.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.tarul.cn/Article/details/gaclhxzta.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gajzqsjef.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gvpuydhxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gtgxcikhy.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gmjotpume.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/ghxqffzuu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/goqjyyokt.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gqfpsmvqe.sHtML


<!-- 参考信息 -->