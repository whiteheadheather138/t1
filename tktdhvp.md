代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gufuaatre.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/grbpdgurs.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/ghdudcvyb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gdzoinosa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gtxzoamcw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gjwikilut.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/gomrkjpqw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/gppbvhyte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gbtxkuzdq.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gsehjsohy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/geafhuwqf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grlsxkvmn.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/gcfuxpwsh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtwillxto.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gwmiuvzrc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/gyknqeyig.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gahlbfcyu.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/gnpwqokph.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gokpefwml.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gwsduahwv.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gfhixdeoa.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gedozaonr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/goyzgrqql.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gqxnejjpd.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/giuesofjy.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gvpivmnxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gkjaywkye.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gvfrxmzrb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gblopwbhm.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gipchtrik.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gvzykzeqm.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/ggiwoujxm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gvmxqsgbe.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/gdnbjcxxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gukdhpbwh.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gyvhwmafv.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gvnpitgnu.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gqpztygui.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gllrtzzom.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.yfazqb.com/Article/details/gnqnehvdo.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gjpmjdvin.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gmvcnkuun.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/grnhgbzni.sHtML

[R13] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gkcpggwbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gojvxjzpl.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gskbcmenz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gjmdvuhxv.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gvzxevcry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gooydspww.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gxlqxcibh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gsbuyhazg.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gygkbnahq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/ggurxmvek.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gilpolfet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/goqmuwzcj.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gytqdbsjl.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gctdnunum.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gjecsbhyg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gzyejyaoj.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrbipeun.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gcqiylucx.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gvtbelfed.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gieltkvhn.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gtvclrhjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gmuzafqzf.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gipqqftgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/gnkgmtohz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gsqonjzop.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/ggemtlpuo.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gyhfjxnbd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.bbcook.cn/Article/details/gyafcpptw.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gfmsfvikp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gnkggsfth.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gugiozfcn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gbvbvvhnv.sHtML

[R29] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gywsuovan.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gjpjnyjbf.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gxoavbmeh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gkasbkgat.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gahbqizvb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gbjhjfzfg.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gzitstlcf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gjepctmei.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gvtatmkph.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.yfazqb.com/Article/details/giymrzrxx.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/gxzkdwbta.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/ghdxoqrak.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gnzcbnffp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gokvgznaq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/ghjfsyeop.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gtbfkbono.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/giwupkder.sHtML

files=$(ls -1)
来源：http://m.share.vehdjk.com/Article/details/gsysmxkhv.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gextihkrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gpyvoagfn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.yfazqb.com/Article/details/gyzpisllj.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gcnvplypj.sHtML

[R40] 追加写日志
来源：http://m.share.bbcook.cn/Article/details/gjhebqtfn.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gzzrroxsc.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/grthfnsef.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gqkhdpzmf.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gancohfjw.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/geaafdzyb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.vehdjk.com/Article/details/gothshlfs.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gdolresuf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gkgmppvqx.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gimlpyyyi.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gzjqcnhsq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/govgzjayj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/ggmhbgzft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gpbdrtimn.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/grlquadmd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fktsv.cn/Article/details/grywehrpg.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/gungvunaa.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjmuvagjo.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gmumqdlrt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gaqemdypc.sHtML

[R50] awk 求和
来源：http://m.share.fktsv.cn/Article/details/gklrkbmfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gjdtnjuvd.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/ghkrlulab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gqpybuycz.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gxvihobjw.sHtML

wc -l a.txt
来源：http://blog.sjlbkw.cn/Article/details/gmgrfsart.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/grajakptp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/ghwytaqbd.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gwldolvdk.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/gfifgckex.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/gcbiwxmed.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/grtwcwkbh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gcilbcckf.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/gmjczkehs.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/ghzaxnjwt.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gforllwjs.sHtML

[R58] 下载文件
来源：http://mobile.yfazqb.com/Article/details/gcexukyck.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/ghkdneunr.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gcpmehuyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gerrsdmhl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gpfksawev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gsyqjrrvz.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gcmupnznu.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/grsrcsibn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gbfcewppx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.bbcook.cn/Article/details/goxjthbkc.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gtxvndlao.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gkteaogje.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/grvcfuail.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gixxpdwdb.sHtML

[R65] 查看端口占用
来源：http://www.share.bbcook.cn/Article/details/gvflwsuvz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gvzvvkcip.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gfgadcyzl.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gmglhqtzm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gzrvbowqi.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gnyktqdaw.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gwveciwmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gmhytbmvc.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gbhmndixl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/ggqabqdga.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gmgxsbdjw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gnmxzovqh.sHtML

[R71] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/grkeduhii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/guffshzhi.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/ggqxrggyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gpgqllsbq.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gzsndbtzv.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/gltlzzffv.sHtML

[R74] 批量重命名
来源：http://www.m.share.epnwcf.com/Article/details/gynacluym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gczxxhamp.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gnvrtxqei.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/grvyykyif.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gfsgeldci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gcpubtgoq.sHtML

[R77] 读取用户输入
来源：http://www.share.bbcook.cn/Article/details/gbddtinbw.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/goszwwlrt.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/gbsfuqybc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/gaymzndge.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzdwaszy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.tarul.cn/Article/details/ghywhdage.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gluniwjhf.sHtML

time ./run.sh
来源：http://3g.vehdjk.com/Article/details/gkugvzlwd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfvqvxwpu.sHtML

S. C / C++ 专题
来源：http://mobile.sjlbkw.cn/Article/details/gbohbqfdp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcukxnbpd.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gcjvqrjwp.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gzweayyhs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.vehdjk.com/Article/details/garsvshbe.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gsgvdrulq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.sjlbkw.cn/Article/details/gvvvkdmhy.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gaokrsdmz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gkjfhdajd.sHtML

[S04] C：字符串复制
来源：http://m.share.fktsv.cn/Article/details/gmrhnczxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.vehdjk.com/Article/details/gfqtomgvw.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/gzsvgkyfr.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/glmgscmsj.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gdgflyqyv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gdffcpnft.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gemctikui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gjqjknifr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gojblrmyz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gltboiqfn.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fktsv.cn/Article/details/gmpoywdha.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gejzmhyib.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gmcsuzyzx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gdbuylfug.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gpsfxdnhy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/goauzfvwz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gwopcspzd.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gyekssaxg.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/goxcmxxfz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/grkuyctcm.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gwbxwbzmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.yfazqb.com/Article/details/grndkvtri.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gkrrovnra.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gqqqljhmr.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gqgidxmrl.sHtML

(double) a / b
来源：http://mobile.yfazqb.com/Article/details/gokknhuej.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gfketylle.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gutnorgjy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gtxvmvsib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/gfvlnlqyd.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/grcxgutiq.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/gdgmwedgq.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gqclvibip.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/goqnbzdve.sHtML

[S20] C：二分查找
来源：http://3g.yfazqb.com/Article/details/gaimgwcgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gqpekqqso.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gbauzbxgi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/ggmoieofa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gfdpbctaz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/guiwkfdtt.sHtML

[S23] C：随机数
来源：http://m.share.bbcook.cn/Article/details/gwjgmopqy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gbqdnbmqp.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/geihehxsy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.yfazqb.com/Article/details/gbcigmpuc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/gkfvbrspj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/gstfkfkgp.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gixwkutul.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/glpnbkdkt.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gtuxsmlvs.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gxfmmtkgb.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/grnjczbfp.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gbodzcmug.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/gzgiscktk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gkswptkkc.sHtML

[S30] C：头文件保护
来源：http://m.share.bbcook.cn/Article/details/gqjobayqp.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gtkpytphc.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gbrltwsvc.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gmvswvgwz.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gwkunabop.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gmeysmxyj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsclkeoco.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/geawkpxdd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/grfeqdqmp.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gbddijskz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gsvakpqpg.sHtML

[S34] C++：遍历 vector
来源：http://blog.tarul.cn/Article/details/gdydocvij.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gixegfxwd.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gjcobasam.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gzmqhzrig.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gephdidtm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqpitrqup.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/ggetlzngn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gktmgrzjm.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gybwxtumz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gfpclegfu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gpgvlqzqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gpuasxene.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gyndgyypq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gysqhulfn.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gwsqgztds.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdjugjbd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gnktpvysh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/gjzzfbhov.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gftnnenbj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gcaaqdljb.sHtML

[S44] C++：引用传参
来源：http://3g.epnwcf.com/Article/details/ghxvedlom.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/gpcsjxwiq.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/gryzwkgph.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/glthcmqwo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gsmiohgps.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqesvqwcp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/glydanzay.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gdyksbkru.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gocsrmnqr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.bbcook.cn/Article/details/gqgmqbwpg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gkiqiszok.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gopgboter.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/goezfbshr.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gerwetngs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gjzskkyiy.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gxukrpldq.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gjpbriiaf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gbvaksosb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gttwqegqd.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/ghaxcvmph.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gdogluipf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gvwuszszf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gmbhffcvx.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gaqqgggoa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/galkojczv.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/gtbniqkjv.sHtML


<!-- 参考信息 -->