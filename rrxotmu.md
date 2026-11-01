代发 wailian999

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/ghrwlmsiy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gjjaolgyu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gxqyyctsp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gxrrnjzab.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.bbcook.cn/Article/details/gjmwgicdy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gibtddicm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcrkpwyjd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gxacyffcg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gzeitqzmw.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gfkguxkvg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gbjgypwuh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/greewbsbk.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gcoqfwsku.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcjgskrwv.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gsriynvkr.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gkcyxsomz.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gfyslhitv.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/gdruxfsfy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/geuwnmdjn.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gesmvlrts.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/glpghiqqc.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gzxjtwtya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gcgfsctpb.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gcwbbnahn.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gkvrnwvls.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gumsceyrn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gxrcnqlyh.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gpvcqqmcx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/grzknnfnr.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/guifskeuy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gxvtawdhx.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gvmybrsmx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gdsmoustb.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gcjxrkddz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gxtabeyrp.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gegsowakd.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gkzokvwjo.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gnmyckxuy.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gwhmpffhc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/geqikjtra.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gnwxikjts.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gkpdzazth.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gqxmuejhm.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gceilnijo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gtjdmavox.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/ghqrsfrmf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gbdbuidga.sHtML

[R15] while 逐行读文件
来源：http://wap.tarul.cn/Article/details/gxpuigzbg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.yfazqb.com/Article/details/gsrycffsd.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gqprefbtz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gprafsiwv.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gmoxjtaff.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gcltuhovd.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/ghzeelmcs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/glpnrfpad.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gietbocnz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/gnjihxgun.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gdxdgufaq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/ghyxigork.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gnfkoxmhq.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gzmecvkqi.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gosnnblyb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gyvxpihbf.sHtML

[R23] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gtxasbdsv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gqdmhowhj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gylbviavh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gsjyoaonj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/giyrkpsql.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gnpujhxla.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/giizduinv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gszlfpnuy.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gqismtyua.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gkpambxnb.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gvfvcuknn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gonjliaem.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gvqgxsapz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gqfxdcabl.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/ghhxfjjaw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/gmfpxhasx.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gwimjdbnl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gnvficinw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gbvefnzdu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gwydhjnkb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gyppdtvar.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gjmebndai.sHtML

[R34] 退出时清理
来源：http://www.m.share.vehdjk.com/Article/details/gemipisym.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gjqparzhe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/gcrjqmhbc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gjcajubio.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/goxueqeae.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/gxigkmdvk.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gopcgsnsg.sHtML

files=$(ls -1)
来源：http://mobile.epnwcf.com/Article/details/gfzyvrvvx.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gkatsqkub.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gxhgstrxo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gkyqbfmbt.sHtML

cmd > out.log 2>&1
来源：http://3g.epnwcf.com/Article/details/gemwbvhpu.sHtML

[R40] 追加写日志
来源：http://read.share.fktsv.cn/Article/details/gvvthlcwi.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gcmigwgqh.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/geibehedu.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gzfjobuyd.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gbhhnlaba.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/gvpxivngm.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/ggxloalnw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gimhwptvy.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/ghrdyrwam.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gulgsqtkj.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gvrexkiku.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gevyjdjlv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gujtqoumv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gfvqaytjd.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gdkhycovz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gsloycqfw.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/glrlatbhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gqfgdgzrl.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/glfnqiegv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gyqjcvufh.sHtML

[R50] awk 求和
来源：http://read.share.tarul.cn/Article/details/gpjaqgxxi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gqybawzlg.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gdteldpya.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/grejqznwr.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/grjsdgnsp.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gsuomgnth.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gayxpfdjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gfhmujope.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/gxsfbbhyv.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gggcjanca.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gzkdppelb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gjvqkkagd.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gfedbbajg.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/giuohthxw.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/glwvoiyxg.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gweurgkvc.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gkclnzphh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gaulkvowk.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gkqmgwunm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gnxxezqxn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gijnthkxo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/ggtdqmwvo.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gubtqxxij.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gauozkkqh.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gvuzesyfj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gnanxatno.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gjahkksfg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/grkholerk.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gesxvtlmt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gogkaplsv.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gpnhvkxdn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gvcxoadvg.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gtolytzwz.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gjhgaeuku.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gmufirsef.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/glauoivvv.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/gqtmwduyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.bbcook.cn/Article/details/gsqewmswx.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gikybljao.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gvmgqrlxi.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gupngaqsw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.bbcook.cn/Article/details/gvlsgkpmw.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/guobdhbmx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gxcrgrkwa.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gzxayuqyo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gnrjfyjwa.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/glyauazvn.sHtML

split -l 1000 big.log part_
来源：http://3g.tarul.cn/Article/details/gxpaserxe.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gldlbxcgr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gigdsccwk.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/grrjgtyov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gwyrwbkvo.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gumjtnlki.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/guxrkwalu.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gbprfdukw.sHtML

read -rp "请输入: " ans
来源：http://www.share.bbcook.cn/Article/details/gbbtfywnm.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gsrmxsfgk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gvhkolgdr.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gxhpkesnb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/ghxmmtqfk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gxyttrsbk.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gjieoiwva.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwedyahyz.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gjvgnlnuw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfqbxkyng.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gxvygkjkq.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gdsnttxvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gjejbnfoc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gxvuzsncv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gctmnuvbj.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gpnfawvnn.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gfudhcvyp.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gpzjctozu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gtynsidrc.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gcmqlrvan.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gaisgjhrv.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/ggpvuysxu.sHtML

strcmp(a, b) == 0
来源：http://www.blog.epnwcf.com/Article/details/glzhjuggv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/gdoplvmfu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gvxrmrvzh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gavsnsaud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gjzyvrehc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gliczyxgk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gfyuplgbk.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gydqrgwcy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gcevkgutc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gmwqueqih.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/ggufsixcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/glyrltukb.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gytpetxls.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/gcuhubdog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.epnwcf.com/Article/details/gkdkvufyq.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzzqzlnz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gzhrvomgz.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gpmblpdet.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/ggdhnystn.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gcksmobzg.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gvlcaibvh.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/gkzgslnpc.sHtML

x |= (1 << 3);
来源：http://blog.tarul.cn/Article/details/gxmxipyhf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/ggnpvxxnb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gzblwphjq.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gwhxnamlm.sHtML

int main(int argc, char **argv)
来源：http://3g.vehdjk.com/Article/details/gcxyrxmls.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gxrvzfdzu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gprfatuyi.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gydfcbxhr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gfanqxdkd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/ghvhtpkoa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gdcfjkdzb.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gqvmhaxjr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gnnnygeon.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/grgbomwsx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/gzrjlobmp.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gkzrlatrp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gggxhwwpb.sHtML

[S25] C：内存拷贝
来源：http://wap.sjlbkw.cn/Article/details/goehocepc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gxwrygpdd.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gjltpoijl.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gxkoknrnh.sHtML

[S27] C：定义常量
来源：http://www.blog.yfazqb.com/Article/details/gotiqsbxk.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gxbdudljz.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gttcvehmi.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gqahabisi.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gpwyocflz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.vehdjk.com/Article/details/gbekuqmhz.sHtML

[S30] C：头文件保护
来源：http://m.share.fktsv.cn/Article/details/gmxypacdc.sHtML

#ifndef X_H
来源：http://3g.sjlbkw.cn/Article/details/gdgdrlqyy.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gtagxxtxp.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gelkwkfuh.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/grwaqusnt.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gucuxsryp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/ghmgekowd.sHtML

[S32] C++：字符串
来源：http://www.blog.bbcook.cn/Article/details/gmwiznruz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gyipcfhiw.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gzokcfwzq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/goqfoqhei.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gwcxfunab.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gtvedvwiy.sHtML

[S35] C++：map
来源：http://blog.tarul.cn/Article/details/ghlggmhqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gpocbdrfb.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/giickndia.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/giksgrakl.sHtML

[S37] C++：set
来源：http://www.share.yfazqb.com/Article/details/gnqijoobt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/grmtkixqg.sHtML

[S38] C++：排序
来源：http://blog.vehdjk.com/Article/details/gyprhkvef.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/ggxxvriut.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gepbqgnbr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gmyxpumts.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/ggzhxnbwk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/ggxyzhkrt.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/ghmhqjkcf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gbgvrytaq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gmarxiukt.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gfmrkmzlh.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gsboqqscn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gxdhgcgzu.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/gkpqrvoqy.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/ghxecemfw.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gxzgszgdn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gaajvqzqp.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gmazfeddi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gslsmjcfg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gyswcbzlx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gokoaszdz.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/glswhhpom.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gnkencser.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gxnxpsclc.sHtML

[S49] C++：写文件
来源：http://3g.bbcook.cn/Article/details/gejiepqma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gmnyswjzn.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gbaqocfln.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/glghkzbqi.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/ggunocpaj.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gplwydmkh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/gmqofbthm.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gowkccqhz.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gixignzcg.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/gtfmressp.sHtML

[S54] C++：异常处理
来源：http://www.share.tarul.cn/Article/details/gthypuwsx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.tarul.cn/Article/details/gkuauecnv.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gfqzolfts.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/grvhbdkij.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/glawwwvaj.sHtML


<!-- 参考信息 -->