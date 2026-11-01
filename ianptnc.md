代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gzqrnivnc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gdeeskgpe.sHtML

[Q85] 数值取整
来源：http://3g.epnwcf.com/Article/details/gcloycuhr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gmbevginp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.epnwcf.com/Article/details/godewmfhw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gbueimhhj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gdwevuvzp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gjbushvbd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gnjpjunlb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gnjtkwjrd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxorcpfwn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gofhyxmba.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gkrwpebmi.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gchftcfrn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gmqgeamto.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwhhofyjc.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gytzzycem.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gduepktxc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/gpvlqkptm.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gfwdqacwe.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gkhxzjeig.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gizddggoo.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gueahmtuz.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gjhhkyigw.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gmnlbjojr.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gsvtrpvbl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gqwradehr.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gnwsovxdz.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gifdqhxru.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gdwizgyfb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gnjurichv.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gqfzpmxsv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gouizqphd.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gjlopfhgg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.tarul.cn/Article/details/ggdocyqra.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gmgwamsqe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/gqttynjti.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/gjgsedaqq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gcezpevha.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/ggzimhima.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gbgldyicf.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/grinrkrap.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gemhilkod.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gkrpuhsgd.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gjrrlftvx.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gsbmiqgtn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fktsv.cn/Article/details/gorhwymlo.sHtML

[R13] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gqyjgvubk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gnnegtnjq.sHtML

[R14] C 风格 for
来源：http://3g.yfazqb.com/Article/details/gguqpygny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gqcviqenc.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gmgpqafdx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gcoyxbclf.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gntraaoms.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gtskhbkvq.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/griosfiah.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.vehdjk.com/Article/details/gvzohdyab.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gbnuabhcv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.tarul.cn/Article/details/gaqhrsqlj.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/grrulbljj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/glqcucqpg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/glbrgefsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gopodifsz.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gzihtijwm.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gudzzplgd.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/giwnxqudd.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gbfmuzmfz.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gvistfdyg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/grojooaje.sHtML

[R24] 大小写转换
来源：http://m.share.tarul.cn/Article/details/grvjwlwyz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/grpwnaqcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gugmzvikx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gduqgdgku.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gjjumeudf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gkhbkznff.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gxibxhljm.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fktsv.cn/Article/details/gbkyfrqnq.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/grkejtkew.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/ghogdzqcz.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gljivpsee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/goirmrdka.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gkymbjdkm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gvaglfgxm.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gutwkzwtt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/ggbdftiwd.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gbizzamme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gibmashrl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gskygqsgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.tarul.cn/Article/details/gtsfjdvfg.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/ggobaxzay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/guybsojjf.sHtML

[R35] 后台执行并等待
来源：http://read.share.sjlbkw.cn/Article/details/gyflksazz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gfilamdry.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/ghkuntmqx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/goexhfmbb.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gmihxfxqm.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/gzfhrwzgu.sHtML

[R38] 管道串联
来源：http://www.share.yfazqb.com/Article/details/gnillhnho.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gbrgmeccn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/gprwvgurx.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/giopwpplj.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gjswnxecu.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gdtersqpt.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gjxazxxpe.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gvtijmyzh.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gtxedoabg.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/gbmoqcifj.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gcgyoyzaj.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/ghybpoqft.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gmtyzbnar.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/ggnawepyf.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gxoofmgvm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.tarul.cn/Article/details/gtfnepskh.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/geocmjipn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/glmiybgtv.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gsafklxne.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/glgeilysn.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/gvijlaxbc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gqzkzquzd.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gggajyhct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gmvlprdbf.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/geuksktec.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gqspgncmu.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gjknowrrz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/gqmmgqcit.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gufrtapyh.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gibbvnuen.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gpoglhxah.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gkocobuun.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gmcpjjces.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gvziohgno.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gcmocmshe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/grkgukggb.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gcrnolhjy.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gzmqoepqq.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gzoewvpvv.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gkaelztpg.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gvwzuxazh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gfaniddbq.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gnaiacpml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gsigcmgaa.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gfrtbxrem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.vehdjk.com/Article/details/gghyjdjzo.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/gawhbbqyu.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/glbonsrlr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/ggyefqrfg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gjhftpolq.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gpcfwzhgt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gyyjnlvyq.sHtML

[R64] 结束进程
来源：http://read.share.fktsv.cn/Article/details/ghgmtcyxf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gjjjkrgap.sHtML

[R65] 查看端口占用
来源：http://blog.epnwcf.com/Article/details/gjsxuunkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gonvgqvlx.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gpacoopoo.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gxifommfo.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gdrudlxkd.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gfhwuzzpo.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/ghcfyoziv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gfhxfkglm.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gnldvrzbs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gsnpmdkks.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gnqbmcaac.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.tarul.cn/Article/details/gtdntjscx.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gptbrlblc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.yfazqb.com/Article/details/gpaidkadt.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/gaxapzrjs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gkkvikfkq.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gzyobvznv.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gukdehkyg.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/glujwkqvh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gzwgeynuj.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gsnlitmqn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/gpiuanwcs.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/goqusqdeg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gidwyytsg.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gamoahexw.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gmbiwzojz.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gxgemesbh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gxxicfkdo.sHtML

[R79] 解析命令行选项
来源：http://read.share.yfazqb.com/Article/details/gckkvnopd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gybxtihco.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/grfgonrpi.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/ggkqyorux.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grqkfgcvq.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gkyxmlrnr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gttvyemuo.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gpxpdafng.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/gyyveroks.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gerdiwqpl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/ghnblogps.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gofxuvaju.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/grtpaqedp.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gvluqodbl.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/glxmppqex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gphwzglye.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gjipxrtyr.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gtszryqtw.sHtML

[S06] C：字符串比较
来源：http://m.share.bbcook.cn/Article/details/gqauwidtl.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gliifstut.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/ghoctlltm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gshssmkiv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gltotxvsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.bbcook.cn/Article/details/gukupkvyz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/ghzxldjqv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gzngwgucf.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/gyvambddf.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.bbcook.cn/Article/details/gjbbrndrq.sHtML

[S11] C：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gjzzmsxdn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gvtxixkha.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gityvcudx.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gibpzcsax.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gxrypxszr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.tarul.cn/Article/details/ggtagtsoe.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/ggsuuupdj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gqesoqzkn.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvlbnltq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gldmoguni.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/ghdpfaeif.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/guboorajh.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/ggmzlocax.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gzgwdfyqt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gmdtkxoek.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/gtpmmcomb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/glpshgcdt.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/gyhjbzijq.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/gybjwwdcj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gzghzctrj.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/ggcvwbksx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gangcarxh.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/gcljuhvel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gkllmmdpd.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gohwfnlhy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/greymjsis.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gwrwszfby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gobptwnpn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/godjopabo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gioliyjen.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gtjqnyggu.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/getuwwtsl.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gbsukhbxn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gwvzbjfuy.sHtML

[S27] C：定义常量
来源：http://mobile.tarul.cn/Article/details/gnsjjpjwv.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gvmdfzjpj.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/gxeyqawsb.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gugqgmahz.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gizyvwfvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.sjlbkw.cn/Article/details/grtevjbwy.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gnhuqstwr.sHtML

#ifndef X_H
来源：http://wap.epnwcf.com/Article/details/gsnddaqup.sHtML

#define X_H
来源：http://m.share.fktsv.cn/Article/details/gomcaaxvs.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gnnqgbwou.sHtML

[S31] C++：Hello World
来源：http://mobile.fktsv.cn/Article/details/ghkctvjpe.sHtML

#include <iostream>
来源：http://www.share.sjlbkw.cn/Article/details/gatgqfsev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gtxjwaapz.sHtML

[S32] C++：字符串
来源：http://baike.sjlbkw.cn/Article/details/gnmxkruuy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gvczudyea.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/goovbalxx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gimipwhdh.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gfeogacct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyprpwzuq.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gqfesloeb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gorldrkgs.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gernbqkyg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gcjxsohlh.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gsxgusvlr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gnidcuiof.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gsxhiqblq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/geoayzdby.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gehamaupr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/gpkcjowwh.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gitcrndps.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gnlkljxoy.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/grhgfamkr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gxjgvdhbi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/ghirrgalg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gzqybjbys.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gjfnkoalh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/gwwfesvnf.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/gmnqhjlru.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghlmlupzv.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/glsozrkee.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/glrbngkzc.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gfmxvcuey.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gjdcfrlfr.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gyzxydlkh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gqyiwhhek.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gjdhrrznb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gsvtereep.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/geunzivht.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gxbetqwhf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gyeoerwzi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gjjpoberk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gzecdxgru.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gikckyixn.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gohyitoeq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gxyoeckpf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gxpunrjts.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/glzpzsakr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.yfazqb.com/Article/details/gxxfprtxv.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gvlcrcasg.sHtML


<!-- 参考信息 -->