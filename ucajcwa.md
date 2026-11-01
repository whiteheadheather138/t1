代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gjdylgzos.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/ghhiudtaa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gojokvrrc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gaohjsafq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/glocmhnqo.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/grdocswba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/ghfwvxeca.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzatiyidg.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gvrtxenzf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvgrbanx.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gqamgskmt.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gnftvzktv.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/goazqqebh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gxefxuhnj.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gedxhxqmg.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gfhsrnksa.sHtML

readonly PI=3.14
来源：http://www.blog.vehdjk.com/Article/details/gpfvkpebr.sHtML

[R04] 位置参数
来源：http://blog.yfazqb.com/Article/details/gzapgivxl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gxyrbrhjq.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gpwhvatvw.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/gkpidezyq.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gjopajakl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gitecudto.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gfmkqtnoq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/ggsaynjus.sHtML

[R08] 数值比较
来源：http://3g.yfazqb.com/Article/details/gwmkhlhan.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gpszmazjb.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gsfsjgncl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gyedwexqi.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/glblplggm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.vehdjk.com/Article/details/gyppjarba.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gkmaolznz.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/gvrurkyxp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gxcrhziqm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gqslikuqo.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fktsv.cn/Article/details/gwycwkvyy.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gskoxwaor.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/goalgzoib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gpahlvpqs.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gtjofhpua.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gbrdmnpxq.sHtML

[R14] C 风格 for
来源：http://3g.yfazqb.com/Article/details/gdyqjtzko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/glykggtda.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gzhwhhkxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gvahobszp.sHtML

[R16] until 等待条件
来源：http://3g.tarul.cn/Article/details/gyzgavgsg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gikxqoikg.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gawjannvw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fktsv.cn/Article/details/gahntmdty.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gtqpysxub.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gjgdxupbw.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/grwnffqmk.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/germfkrfs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/giyzomnrf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gaguytema.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gbzvrqhcp.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gxttduvgi.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gkcdiahxy.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/goazydefo.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gzqfjqtvq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/govshqkqs.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gygvwdxzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gqxipdqnm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gttixlwql.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/gjhscrjnz.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gahfnymbi.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gpbadzmrx.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gyshonctf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gadhvfedf.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gusfgjqum.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gbqkiyvie.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gouopovnj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gsvumpmaa.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gcpjjzeui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/getxnwech.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gjytckppq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gryjaeybf.sHtML

[R32] 参数个数校验
来源：http://mobile.epnwcf.com/Article/details/gwxqimxqv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/grsptooei.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.bbcook.cn/Article/details/gabrlhvpa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gakucfvxm.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/goctxclja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gtnuxgzws.sHtML

[R35] 后台执行并等待
来源：http://blog.vehdjk.com/Article/details/ghlxhtbnm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gsmarlede.sHtML

[R36] 并发执行多个任务
来源：http://m.share.bbcook.cn/Article/details/grultbdzx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gkseqvjmf.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gfyxqnqlc.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gueffcwax.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gpkkwirwd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gzjpvtius.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gvonrbdpa.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gxdjhltcx.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/ghrleevuk.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gynajioiz.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gibaeouag.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gqloecfdr.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gxjuawzfx.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/grtqydpha.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/gikygbjpl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gstkpnbkq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/guofrlkht.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/ghswawyfd.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gtshaqvdc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/guuyhfkhu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gmqnkugff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gzleiaaca.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gmwzgveag.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gbckhkuvo.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/gmmykupkd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gyeysjiub.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gfhgigild.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/ghbtrkypb.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/guurkbmcb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gjoochpxt.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gvfpmulpz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/ggcfaizcz.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/gbobkodun.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/ghjfyblji.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gicrwntat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.vehdjk.com/Article/details/gxuiybubv.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gcgdexjko.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gjvzbillg.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/geslenjbg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gxtomtwek.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/ggqcyuxed.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/galfjbmvy.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/gogzjsjfq.sHtML

ssh user@host 'uptime'
来源：http://read.share.yfazqb.com/Article/details/gjbttciwj.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/gkpttuqhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gofdxivbh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gycltokcc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gjdepzvzg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/ghemxajbo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/grjqhdxxk.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gjbpzzegz.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gpwewpsem.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/gvijyxxxm.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gpwwyyqps.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/goptlaznv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/grqylqemf.sHtML

[R64] 结束进程
来源：http://wap.yfazqb.com/Article/details/guvdmnmsa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gvxqcezqh.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gvzfjkdod.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gqekyfgbu.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/glsfptsha.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gilhfujya.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gdkzlxzlg.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gwumtbckf.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gztvpfbmn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.sjlbkw.cn/Article/details/guwterkfd.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gmaqxnjdc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gkkpwrmvb.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gjkhdtalo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/ggdssfdue.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gcumfsurp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/ghpirsaym.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/ggemuwedr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gawwjdbgo.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gikcihmiq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/goddmrvry.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/glelozdun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/gjtkwqcjb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.epnwcf.com/Article/details/griwdadvh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gssdzjyro.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gyxxemffz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gavpevzww.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/glqavodbo.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/glzybxsxk.sHtML

[R78] 交互式菜单
来源：http://read.share.bbcook.cn/Article/details/ghtrdkegr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/ggcmeglhk.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gjiqxzxcz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gtfbmbofk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/gtwqnrxps.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/ggaijrgpk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gczagvkrc.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gjvgpzcri.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goycgrrlp.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ggdcccrba.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gizuoyaot.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gadcatieu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gwqblfrws.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gmnvkxygn.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gfahakyfl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/giklikzoy.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gzimhbzof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gkjhndiiz.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gkyzshwhq.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghnspfabq.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gxanuqavm.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/grwffhfka.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gfqiidmnp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/ggjgjuvjf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gwrhfnuvl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gbuuwxjdo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gtmdkkbji.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gjdfibpyr.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gmyiqoehf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gegxhzoop.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gwudodvsu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gudaulxlz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.yfazqb.com/Article/details/gpxfltsvk.sHtML

fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gzyytjuti.sHtML

[S12] C：写文件
来源：http://baike.sjlbkw.cn/Article/details/geojbfira.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/gtnsbnooo.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/gqooikmhd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gutoahggt.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gxqvyjpos.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/giayajlfn.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/goqfxqpub.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/gmoukgjxz.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gkrevjfid.sHtML

x |= (1 << 3);
来源：http://www.m.share.fktsv.cn/Article/details/gfygyjtge.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/geupiesiq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/gijggorfo.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gnfslwmft.sHtML

int main(int argc, char **argv)
来源：http://read.share.epnwcf.com/Article/details/gfgwlymog.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/glyfjuyze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gdeipsqtr.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gztdutnxo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gwwnsybpx.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gvvqriaqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gctdslxxp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gfvzzjjke.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gfefnzmfp.sHtML

[S23] C：随机数
来源：http://read.share.yfazqb.com/Article/details/gozcyojtm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gcenwqnhk.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gbfqpruwg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/grmbibyah.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/geyrybtxo.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gwgniruht.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gzqbpjyxx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fktsv.cn/Article/details/gzqrdeiys.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gljcvblkx.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gadkcwnzy.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/ggemrqdsi.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gijqweyuu.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/glxrkpjfe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/grxtgdxif.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/guitidztg.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gtoqzovyy.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gwjqvidoh.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/gctnhdaiu.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gsqjrqtke.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gsxcjyols.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gqduirvvz.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvxwsxcsa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.sjlbkw.cn/Article/details/gvbmneumu.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gswtvdwpp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.vehdjk.com/Article/details/gnmyzxirg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/glrzwfele.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gpwscyhvm.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/gmjhuoffh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gmfktkgiy.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/geddtodbc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gzlbqttdu.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gjofzjudj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gmegzppqm.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gufxffezb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gsazixeil.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.bbcook.cn/Article/details/gqnoratde.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/grbmbxglt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gfqwwuzdv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gdahstygn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gcuxhewau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fktsv.cn/Article/details/gqbngkltx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gutzzyydf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gazbeiojl.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/gxiobyhyd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/genpdfrfu.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gsbvsbmvu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.tarul.cn/Article/details/gcohupmtm.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gbmzhosmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/ghlyqqxtg.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/gtlfuikjj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.bbcook.cn/Article/details/gsjztxptv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gyjccenuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gckmvuwjp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gceyyfejz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gcoxvdygh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gvrifvdej.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gwosdrehg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gvompajqs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gwqhdfuam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gxxzkcvay.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gzbkaovgp.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gwxhyxicj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/glttlgymt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/geayfnoby.sHtML

[S53] C++：移动语义
来源：http://www.blog.tarul.cn/Article/details/gjucodiqi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gjadjmnrp.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/gpsmnuoej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gmmoivknk.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gmihlpcuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/grpiefydx.sHtML

[S56] C++：optional
来源：http://blog.epnwcf.com/Article/details/gpdkutyjz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gdasvmzcb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gtevgzsti.sHtML

constexpr int N = 10;
来源：http://mobile.yfazqb.com/Article/details/ghxfknumc.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gixofafhe.sHtML


<!-- 参考信息 -->