代发 wailian999

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gzzozmlwu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gazwtnpax.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/getrbclfz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grlkdpnep.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gppiragcf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gphzgsmgw.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gfsxormsp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gtsrhopli.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/gnipudmwp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gxcrdaqeg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/gdyssxnwg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gywczqxmo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gwtblwehr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gsgpnozee.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gohurlytw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.tarul.cn/Article/details/gvwmvavmn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/guwiinxqb.sHtML

[Q90] 生成序号列
来源：http://www.blog.fktsv.cn/Article/details/gihrokbvc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fktsv.cn/Article/details/gqfvmuikf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqmgngcfg.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gsjhendrl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grznswubx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/goyriyzid.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gbegsqowb.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gsgkbuvnn.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gcwfmmrss.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gfcfdfdtf.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gaqauffql.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/gtdwygxmj.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gfpndinhb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gwsmgeczi.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gehiiknex.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gnevexlvj.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gnltxbtxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gekwfdjgs.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gtaqfijkw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/gxqmeshsr.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/goiqazvje.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gclnizpyt.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gyzchfpuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/ghzotjluc.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gkpzapymn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gsuqxddsu.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gzenopnkg.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gposnjqqh.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gixvhecds.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gojxgwzzh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gueodljhn.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gzrlieuxx.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/gultlzbdi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.vehdjk.com/Article/details/gvzqkzplp.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gfzzpyvnr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gtpytewmc.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gtlkwwbgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gxgtmbmhl.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gwqhbwnko.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gufttifll.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/giealjdhk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gfimmmprj.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gfxtqqudb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/garxehjtk.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gehukwvue.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gvgabmycb.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gscfrvocz.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gwhdljzqt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gteaylygi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/glmfhrjsz.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/geesqjdnn.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gyaodrltb.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gsybngajl.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gnjyodfwb.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gluuxjjne.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.bbcook.cn/Article/details/gqjgilonk.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/grknaxrts.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.bbcook.cn/Article/details/gmfdiqnlu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gafboryrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/guwgqhzpz.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gcqybnpgx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gyvqovuug.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/geaqigtwu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gfhmexavo.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/geyxbtmjm.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gfamwosui.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gjiiiwude.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/goilhlnnh.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gieumdjup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gqiikaqqe.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gpdiwsxne.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gjxnozacl.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/ghotuvfku.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gobgjuesr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gunniwucn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gjcxhelbq.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gdmmyvlwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gblrrfbth.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/ghttiajve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/grtcenkhm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnazzarh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gpcclkytu.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gagxdagjy.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/geefagsem.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gxynjfsts.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gvhqflfvw.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gxosvympm.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gjpvcomqz.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gvqynizhc.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gefutyyqn.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gtzotewvj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gexvxbtvy.sHtML

[R42] 输入重定向
来源：http://wap.epnwcf.com/Article/details/gncdvviof.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/gtrwjippk.sHtML

[R43] 按名字查找文件
来源：http://blog.epnwcf.com/Article/details/ghjnjsysn.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gofokhfyo.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gopfrrocd.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/goczlnaaw.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gxvuwxdvl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gtcsjakyi.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/goijufkmk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gjarpxway.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/gycduvdcx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/guarnwamc.sHtML

[R48] awk 取指定列
来源：http://www.blog.bbcook.cn/Article/details/gktmnqbkq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gkymvffhy.sHtML

[R49] awk 带条件
来源：http://3g.sjlbkw.cn/Article/details/gbrvqmttu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gildityxp.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gtdidujzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/ghkrszviw.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gwhwmhpmv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/grghshemg.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gkrgqyxic.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gwdpcdjby.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fktsv.cn/Article/details/glfxkfogs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/goprtktxj.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/guzzbqyvc.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gcjobkifq.sHtML

[R55] 压缩与解压
来源：http://blog.epnwcf.com/Article/details/gsnawhgdq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/gqvrsezft.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gpdhvmtvx.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/goqwjygis.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gtpphyfpu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gjwoxdvwx.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gtltkalfj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gvcfxtrsp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gkoseoqwm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gzalafqme.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gzawbqocm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/ggiqemikc.sHtML

[R61] 磁盘占用
来源：http://baike.yfazqb.com/Article/details/gioljueyj.sHtML

df -h;  du -sh *
来源：http://www.share.sjlbkw.cn/Article/details/gpowickcm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/ggvblcyzn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/gxlfzumzw.sHtML

[R63] 内存与进程
来源：http://m.share.yfazqb.com/Article/details/gadfrypkx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gifjpxksq.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/ggwdnjshe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gjwfukois.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gjovfgvfg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gpqfogvtm.sHtML

[R66] 定时任务
来源：http://wap.fktsv.cn/Article/details/gpsjcqerf.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gwnofejpe.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gmywusqgs.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/grpqvkmcj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gxtstpzhe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.vehdjk.com/Article/details/gtjkjbjrv.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gfetgeuof.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.tarul.cn/Article/details/gklmsnjpp.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/gmzjxtkjv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/ggktecnyw.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gfhdykwwx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gjyheppvx.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gdmxhwkru.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gcsqiugsj.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/gczjfqcrb.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gvglbcuyd.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gaykhllwm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/ggfudpnym.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/guuofdqkt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.vehdjk.com/Article/details/gldvcnmew.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gnqzvlivs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gjactikng.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gijuibwrq.sHtML

read -rp "请输入: " ans
来源：http://mobile.tarul.cn/Article/details/gjpdecpjn.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/gtpxocxea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gqzrirwzo.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gcfgorbqd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/ghggjwzpc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gpfadhmcw.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/golsgvczx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvjnvclkw.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gjksfinqf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glhnbndcd.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gndthlund.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gnpduglzf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gyqzhqvqg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/goeneytfk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gominlrwg.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gjlhiwdzo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gqcvpilgg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gvzicunfv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gahwkzvhy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gwopidzhe.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwehxyauu.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gzdsqoduh.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gxccakqtx.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gjuovwkmh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gaoimquzv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gvfjwzglw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gijyjfqxg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gketgjbwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/glhpqtchi.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/giaqdtrei.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gdsvojcrf.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gagplsrgm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gqyguqcvt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/glkhdlbuu.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gohpsxmlc.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gfawzwsgu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gthkpnwne.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gaqevjalj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.bbcook.cn/Article/details/gzgtowypd.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gynbdqawt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gmfyabdtx.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gxwilbejn.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gocuonebx.sHtML

[S16] C：位操作置位
来源：http://wap.tarul.cn/Article/details/gzminmngr.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gfbptzrch.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gxyacdnwp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/ghhfkbcqs.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/genmaronb.sHtML

int main(int argc, char **argv)
来源：http://baike.epnwcf.com/Article/details/gmiaenhxj.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/getkzuszu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/ggbblkkvr.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/gguadoeuo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gaoyicgoj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gznjpyhmz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gwiojxito.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gzddridvl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/goilknkxa.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gfkhjhhzj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/ghwvtyenl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gczwiqarc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gzmcqadqr.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gghbwoewq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.tarul.cn/Article/details/gndxxjbma.sHtML

[S26] C：内存清零
来源：http://read.share.yfazqb.com/Article/details/gczqtdmjm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.sjlbkw.cn/Article/details/gehwwbkss.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gidltigjm.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/ggyucugeo.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gvcjxypmb.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/goqpqgsen.sHtML

[S29] C：变参函数
来源：http://www.m.share.vehdjk.com/Article/details/gcgcolbrk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gwwahlwoy.sHtML

[S30] C：头文件保护
来源：http://blog.bbcook.cn/Article/details/gxdvvxjax.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gqbmnuyra.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/ggmstmbfp.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/ggnouagcq.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gexonwvow.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gvvihhgqm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gacmqmave.sHtML

[S32] C++：字符串
来源：http://wap.bbcook.cn/Article/details/ggbuywujv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gttyutjup.sHtML

[S33] C++：vector 增删
来源：http://baike.epnwcf.com/Article/details/ggmhoxjlk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gqwgwrkjw.sHtML

[S34] C++：遍历 vector
来源：http://3g.bbcook.cn/Article/details/ghlzqearu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grwtsbbzy.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gbwvkdpys.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gfhsmohsd.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gobldqsym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gmojptksd.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/gzlytvvcs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.sjlbkw.cn/Article/details/gslkvwcgh.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gliuxwyzg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/ghmnwrlux.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gwsrsadix.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.tarul.cn/Article/details/ghbxnausq.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gamiwthba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/ggyrktaum.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gdhsgzooa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/geagtmmds.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gwsguvyvc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gihdzcubw.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/grprjcidw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gerzyvwwh.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gffbklvlq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.tarul.cn/Article/details/gwaeqrjal.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/ghufejzis.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/girclypbg.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gsnxynumk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/glkzvzmcf.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gzineycvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gbbivyvyw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/goibhyajf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.sjlbkw.cn/Article/details/gegcgjdpn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gjctsfxet.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gjqyelupy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gldkdboge.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gufkmzits.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gtrrrqwdb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/geiufexba.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gzwatzydu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gthgdtges.sHtML


<!-- 参考信息 -->