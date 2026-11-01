代发 wailian999

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gcpajxqpd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/grradotcn.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gmutnthih.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gdhxnxgma.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gkkrcxbgs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gaqmgybit.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gpoxerlui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gznpsbttu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gngawsoff.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/goboeobvj.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/ggfvjexox.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gazpusvlt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gofoakzol.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gevnyzsur.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gediqftsn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.tarul.cn/Article/details/gcbxlvsbi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/gypjcrchi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gdpcsvpqe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/grplxjenj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gpulavvbv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gkhfjnjso.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gdwteounj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gyshukikz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghzbxzclw.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gswqcddvp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqlqcotjg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gpzqjwvuw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gvouxhldf.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/grcrlxxue.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gvzoebqna.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/grslnhmpv.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gljykdhmh.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/gfcsgwoxr.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gfyibvtxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gdkvhwwjg.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/ghlhumdar.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gftkovcbn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gmcrrojzf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gkjkwebni.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gaxtffgam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gzyxaqkee.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gyinanfga.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/ghesixhvm.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gyxrpzajl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.vehdjk.com/Article/details/gofwpypko.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gmmmywzti.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/ghlujearg.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/gpbqrsqly.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gwcjpzrjp.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gnjiibwmu.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gvpfgwudo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/gzeappswm.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gfpcpytqs.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gnesekrdj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gegjmcdis.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gnruxxgpq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gdngngowb.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/grwcygkis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gjbgiyias.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gckoxettl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gddwbojuu.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gkuddhcos.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gtdwwtqra.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/ggzayaalh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/grlcmcpft.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gnweygryw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gfmpehfvz.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gnsaqhguh.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gxqjizvca.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gfrjgdvvs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gysmjabdi.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gwlhbyqwz.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gkyccbyuw.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gnrutwbvz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/grjotpmpw.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gzpfvlbib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gfsfrapro.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gyfxmquxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gcixuhlqw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gkrvsrzea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/gsvsduuby.sHtML

[R26] 命令替换
来源：http://3g.yfazqb.com/Article/details/gufjuqowx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/glkupgayd.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gzswwdwox.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gqtjzgrxc.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gflwbhupg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/gjyvtiwjh.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gnyiclsyw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/grzlttgha.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gqhacmkjf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gbimayhrd.sHtML

[R31] 局部变量
来源：http://read.share.fktsv.cn/Article/details/gkhpiezsy.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gttfyjnei.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/gucsldoul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfnmrkwo.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/gnjqxhryf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/glgokxhuh.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gevujgdcb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gzpizylsx.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/goxxfchgu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gntahtwhq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gfbzlsmhy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/grhcwpqmw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.yfazqb.com/Article/details/gzntfnske.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gudmzyjcl.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/gltpwhjel.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gkkiglslq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.tarul.cn/Article/details/gxodovpoo.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gebwqnbjs.sHtML

[R40] 追加写日志
来源：http://read.share.epnwcf.com/Article/details/ghureahdf.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/gqaxeewzs.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgftizjk.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/ggonqlyzd.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gjvplrdlg.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gekwlwzyh.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/geprffvjj.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gqtzvrkiv.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/guehtuoat.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gzeyhgthy.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gzzfakmmh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.tarul.cn/Article/details/gkjdtimfe.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gjybaccop.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gdnyrylnh.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gkuycakrq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gkbhnbrlx.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gdtlddhaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/glaejitwo.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/ggoigtsll.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gvnabeoxm.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gzhiweqkl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkvyvowji.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.bbcook.cn/Article/details/grfjhlenx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gghidtqlc.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/grrnakwck.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gmqwlgmgs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/garxjekjk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gkrptkrhn.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gtsxgjbsf.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gsirteozh.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gdnjjcwhq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/ggddrjeeg.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gzgavgfez.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gjjkyofii.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gvexgajvf.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/ggjtiohka.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gcohvifxh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gxtzlquwz.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gfnaenlwd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gohskrwqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gzdvzcnmg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gedhfwmtn.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gdqxebsep.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gtyrjgxkf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/gmcfldacr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gksdlbwoq.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjqcbzkl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgjhocgw.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gvpxmtnqy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gsigmzlyg.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gggeiuawl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gvziwcnlx.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gxwzdiyay.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/ganpvvopj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/glhsnwujy.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/glebrikaq.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/genhhbvrq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gqtvpuafh.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/glxllzisw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gbtnxbryn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gshnjybip.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gdpfdtdka.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/graektrtf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gayakzuft.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gwkwfaafr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gaguunzmg.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/gkdwvrkul.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/glsckygme.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gzseprzst.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gnktrsoob.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gupgnunor.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gesxyipds.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gcztxmhrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/grycuzmsh.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gimufvedw.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gsknwxrjy.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/gqvfosqqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gtpdluplr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gwubzvyge.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fktsv.cn/Article/details/graqxopet.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gkbtqjilr.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gdhcxtizb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grtowlsxt.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gckuvwslg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtwblonzp.sHtML

[S01] C：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gqeqilsfd.sHtML

#include <stdio.h>
来源：http://read.share.yfazqb.com/Article/details/gpmufazqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/grqfbfant.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gidyjvosm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/geizpbqqa.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gfhdcuigx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gsygeqcfc.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/glfjdcsod.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.yfazqb.com/Article/details/ggtwrsyci.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/grwjapgon.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/ghznliryp.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gxfutnlnx.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gxvoitmva.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.tarul.cn/Article/details/gwkmxnezx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/ghsfmomgc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gqhmvcmoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gguqagcki.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gnibtnyam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gmxboqazy.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gelzkesyb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/grfcdzfno.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gvrjyzbtn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gveurzswm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gstjcybql.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/ghrjsgrug.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gczwunvcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.epnwcf.com/Article/details/gkwaphpse.sHtML

[S13] C：宏定义
来源：http://blog.vehdjk.com/Article/details/gejzocjkb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gddeahlmr.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gpagrpsxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gqgbcmots.sHtML

[S15] C：类型转换
来源：http://blog.epnwcf.com/Article/details/gpgvmvirh.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gifshbcms.sHtML

[S16] C：位操作置位
来源：http://www.blog.sjlbkw.cn/Article/details/glvavesbr.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/ggqilzjzd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gxcdqobyw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gldtyuadh.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gijgpydpe.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gshtoazpm.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gohtkqqgx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gpwogzwlt.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/grwrfjych.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/ghzownudh.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/ggckjkjbz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/ggxsqhqyf.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/grxizgbdw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbabphoja.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gctfbbvmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gtxwjvcpu.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gjyipnrwz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gymcosdde.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gfljobaib.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gojpgvwdm.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gfsfqmsjr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gfguuafji.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gkofxzlrm.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gjietaozb.sHtML

[S28] C：静态变量
来源：http://www.blog.yfazqb.com/Article/details/gytsjopcm.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gcmeiliex.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gtmiipwxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fktsv.cn/Article/details/gjlivhtsx.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/grkuknpbk.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/ggmvdidre.sHtML

#define X_H
来源：http://wap.yfazqb.com/Article/details/gcmqzaipr.sHtML

#endif
来源：http://baike.sjlbkw.cn/Article/details/gctnosgep.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gqjeleqcp.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/guozfcmzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gftoracmt.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gmfibwnzh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gsoavybwq.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/grmztczxx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gzsvosamo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.vehdjk.com/Article/details/gowobfdaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/giuruvxlv.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gwwudgsmx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/grpbfilme.sHtML

[S36] C++：unordered_map
来源：http://www.blog.tarul.cn/Article/details/gkoyxktvh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gpalisian.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/geshvfxav.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.vehdjk.com/Article/details/gbjjbyywd.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gyuqezabr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gfsrndjdn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.vehdjk.com/Article/details/gizyhguon.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/ggjmhwrcq.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gpkgwahnp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gyrxfzlhd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gdghneite.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/gjlwvyuit.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/gxplekwon.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/gljphrthe.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gjcbenstp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/gneghpero.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/gwiowqeqf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gmnfwtdjt.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gvdfqywim.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.tarul.cn/Article/details/gsktuhpfw.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gsjjtfqua.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/glbpgbuxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gswcuhtfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gutqjexkk.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gdkqbhkzu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gzcwrutgk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gnwldipqq.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/giraafwwn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gtyqpcgkm.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gomlarxmo.sHtML


<!-- 参考信息 -->