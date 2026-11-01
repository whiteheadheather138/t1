代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.m.share.bbcook.cn/Article/details/gubtfrxcf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gchbdouna.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gbdojziwk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gzffkrros.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gthiagqus.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gkmzstwqh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gluswavvt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqfcscnwi.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gtrckvdtq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gupbewvxa.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/ggtuvyooo.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/grzwilibo.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gtktyohgk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gikiqrpax.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/giuctrhfg.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gjyjgbvhp.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gnfyqkhyn.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gcktfttdi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gyeafoadv.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/glintreqq.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gospfcljk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/guofiwxxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gclreyqqh.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gxygngtqo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/ggyixmcbt.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gvutxijoz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fktsv.cn/Article/details/gtazxnhmg.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gmbeuwvcn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/ggywmqfef.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/godlkiuos.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gulkhkopa.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gxtgeufqa.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gpmctxhiu.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gapnvlvfh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gsoxeityk.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gkduenvko.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/guqpboygq.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/ghcflksvd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gvbuzyfah.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/grclfaykt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gpijmvrbw.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gxztynurh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/ghifzycqo.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gnikmurhy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/ghjrvwwpa.sHtML

[R16] until 等待条件
来源：http://www.share.fktsv.cn/Article/details/ghvpnyztt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gpxiuijga.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/gebpajqzl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gwlwlxmte.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/gjllaoxjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/grxznbfkg.sHtML

[R19] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gntilqpwz.sHtML

echo "${#arr[@]}"
来源：http://mobile.vehdjk.com/Article/details/ggktksiil.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gznsfeagh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gltspvvba.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/grmdvqpno.sHtML

echo "${#s}"
来源：http://www.share.epnwcf.com/Article/details/glukufwcd.sHtML

[R22] 截取子串
来源：http://baike.yfazqb.com/Article/details/goeifneuj.sHtML

echo "${s:0:5}"
来源：http://baike.tarul.cn/Article/details/gsgbsuhud.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gnbxjvujj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/godlidvog.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gatlqetrl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gpdjvekct.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gkroacnni.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gbjkxsxei.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/ghvukwmgc.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/gyqarmycu.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gzsqbyrhj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gknxrbvmq.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gjjphaadu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gebzmfitc.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gvrsixkwj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gfjevponx.sHtML

[R30] 函数返回状态码
来源：http://3g.sjlbkw.cn/Article/details/gozqbxgrg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.tarul.cn/Article/details/gafdjhrlp.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gmryqbdkq.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gntctccbj.sHtML

[R32] 参数个数校验
来源：http://www.share.sjlbkw.cn/Article/details/gkqxjhfcj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gqulmaaza.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/ggoluxbdd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/glqxwmztj.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gftissuwz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gcyahfvzk.sHtML

[R35] 后台执行并等待
来源：http://baike.sjlbkw.cn/Article/details/gzcrscetq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gzwwnbsvk.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gbywtzapa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/glbscmelc.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/grcrujyoh.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gjwjmtycc.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gsibdesrx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/glmomtdlz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gqydkgsft.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqpymgwe.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gezeohjra.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gvygyqnbq.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gialnebxv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gyypcneud.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gebfsrorv.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gvaylfigh.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/glicrdrpg.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gfpyznyfp.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/grdezaivk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gslmtnxqw.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gtuogwkot.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/ghfiticsy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gjeovlbna.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.sjlbkw.cn/Article/details/gfhavubgk.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gpeduvsut.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gqcwqpycl.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gobxcpfqx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gontpowlg.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gyrkvpsmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/geiknjiyq.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gmguypqqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gfbhllntr.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/guwzvsfom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gszpghpul.sHtML

[R52] 统计行数
来源：http://www.blog.vehdjk.com/Article/details/gujarakfr.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gntqflytn.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/gvtflukuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gxzltwqqw.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gyqggsicy.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gtvvicotv.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gqobdjlbd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gqdbzvzkf.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/giriawxhp.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gajxyenal.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gwboxdhum.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/ghnwfpphb.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/gosdkigtg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gzhcfcgsq.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gxduhnaje.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gqluhfitq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gkrgxfqvz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gzjdymcbo.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/gnacsuzbp.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gjqgbsuvs.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/giffvzhtk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.yfazqb.com/Article/details/gifujqdhn.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gjiofuqlb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gqwetmbfo.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/grpkwszps.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gpgqfrnru.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/glnnlxrqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fktsv.cn/Article/details/gbnjtohjx.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gxhhxbmnb.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gjoapmbfc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gqunnpnhp.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gxsmesxbz.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/ggtnpukxi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.yfazqb.com/Article/details/ggmdssuej.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gulppwcub.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/gdkldwkip.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/gtoqupjhx.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gcdoogmfn.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gqsqzbdxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.epnwcf.com/Article/details/gicikfsbp.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gqhengxyf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gwwmsrtgg.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gfmvahokd.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/ghwizmsij.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gdhunkhjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.yfazqb.com/Article/details/gncfklahh.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gycaemzua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gzkathmli.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gfbicdeeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gzwfbrorm.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gwtjbzrus.sHtML

read -rp "请输入: " ans
来源：http://www.blog.epnwcf.com/Article/details/gjoiqbyka.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gxajnjlqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gpvljzdvd.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gxptcljsu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gylzwgirh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fktsv.cn/Article/details/gndbjyrtz.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gkfomrmao.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gieqpclhb.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gdpkhhvym.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcoabxovy.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gpnrhpngl.sHtML

#include <stdio.h>
来源：http://wap.vehdjk.com/Article/details/gcabzasvv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gpcziyung.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/grxgeywvj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gezrgsneb.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gzqnoxcsa.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gopkfebti.sHtML

[S04] C：字符串复制
来源：http://wap.yfazqb.com/Article/details/gglrwqlsl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gxzyvnvdy.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gkylltnhk.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gvmxgrbem.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gorpfzuop.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/gquogytjr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gnjrjwcgj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.tarul.cn/Article/details/gafdbjdjc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/grfasgnhd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.tarul.cn/Article/details/gfpdjjazg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/grtsbiemi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gbntloamf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gzgivrjdf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gqukmgmep.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gpkqdxrst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gkqmhzlex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gpcsezluu.sHtML

fclose(f);
来源：http://wap.sjlbkw.cn/Article/details/gdnzovfun.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/gtazezhiy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gyuxfnfvf.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gontefpzf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/grqtgmsjp.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gcifghrhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/ggmhdlrim.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gtjdxyxay.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gzwiqjoss.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gkoslqfrw.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwzrbdrtp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gpovjchpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/gihembwqo.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/goajrzfjd.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gvfjxikza.sHtML

[S19] C：快速排序
来源：http://read.share.tarul.cn/Article/details/gmsurbrya.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/gmqeokfnp.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gltpwpiqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gbuwacwxz.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gfurvcifz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fktsv.cn/Article/details/gszfeceiq.sHtML

[S22] C：字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gyfhpodsw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gizfwxlqf.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gwqrrofrd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gklgibpvt.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/ggojywcap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gqiuosgiu.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gtttgvqrd.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/ggdjrbjte.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/ghrgchdzb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/grpiparzg.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gbgsdmbrg.sHtML

const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gjnqrjrow.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/geqpnymzz.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/gthvjxygp.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gxzsgarct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhuqllfg.sHtML

[S30] C：头文件保护
来源：http://www.share.epnwcf.com/Article/details/gguepbyyc.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gyplruhsu.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/goxjsjsfl.sHtML

#endif
来源：http://m.share.vehdjk.com/Article/details/glzvgyxkl.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gsfwptclz.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/gqobthibo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gltxbgpms.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/giohuxzsm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gulavoowr.sHtML

[S33] C++：vector 增删
来源：http://www.share.sjlbkw.cn/Article/details/gabrgsqnn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/ghdrfrkvr.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/giqiqvvcv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gsrgsdgfx.sHtML

[S35] C++：map
来源：http://www.share.yfazqb.com/Article/details/gkdjgwcna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gjftbzujs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/glnqvzzxl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gndsbpjau.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gfwllfbfc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gnxyepvev.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gnqacbtit.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/gevqyswfq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/ghmuwnnqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.yfazqb.com/Article/details/gtyavhybf.sHtML

[S40] C++：查找元素
来源：http://blog.bbcook.cn/Article/details/gfjmnrktu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gopxrwqed.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gosibmfrb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gsyiyzkve.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/gkamsixhl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gfaatesfy.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gvqbqpjxo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/glrfxfhgp.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/geymjzmpo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gwysnknwr.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gngmuxwfw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gixnkuuak.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/grvaihefi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gcgsuyklf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/ggfqhwzol.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gejhmoxpm.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gobeoynor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gaowpkdag.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gcqjpkkka.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/gnrtwrrju.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gqofhpuqx.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gadoaxsrl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gytqvlbms.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/gauwsdmah.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gaajlzafj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gmodgtyiv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/ggadigldt.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gnohgywbl.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gbylxonin.sHtML

[S54] C++：异常处理
来源：http://m.share.epnwcf.com/Article/details/gcthhznzi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/gqjdsgerz.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gzefwuoux.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/grupiafzi.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gqsxylqph.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/gfaqxwvto.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gqpdwtksg.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gwgnwzyhe.sHtML

[S58] C++：命名空间
来源：http://m.share.bbcook.cn/Article/details/gndyaslch.sHtML


<!-- 参考信息 -->