代发 wailian999

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gjwqdkyhf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gadwjmlho.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/gfdhkjjof.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/ggzdjuknl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/giwjdncij.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/guzxgzzsi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.tarul.cn/Article/details/gxppvdcyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gretjvpio.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gkmpdltpd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/grwlezcpr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gbqbdsqdp.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gfnslqxnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/grorwycsb.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gzhxjdmst.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gdcgsedoe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/geyjfvsst.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gzdnlldpf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpiquxewz.sHtML

[R01] shebang 与严格模式
来源：http://wap.yfazqb.com/Article/details/gkotmcjyz.sHtML

#!/usr/bin/env bash
来源：http://blog.yfazqb.com/Article/details/gkdonwshx.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gxkffneqp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/giarbxqok.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gaosumraw.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gfdgrekbs.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gsbupiqmr.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gdnytaivw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/geangraub.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gzdjbwajz.sHtML

name="${1:-default}"
来源：http://blog.sjlbkw.cn/Article/details/gutwbjddg.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gtmoackhw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gpftwedtb.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gyhzumccf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gkdjdmmmj.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gopchxkyz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gsillabtb.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gsiyaukuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gxwvqtmfz.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gnqobutqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/goysrnqoi.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gtsnpffln.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gshtotmrs.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/ghxsegwqz.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gcvbcxvrm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gmrwnsbpu.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gzomqfpzy.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gzjslvano.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/goxkfacpp.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gbponmsqg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gnhbytmxz.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/ggbphygqw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gtjkglftv.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gyjximslt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/ghkcswweg.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gpfqtapjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ghjkhcfod.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gfobgqisn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/gzryodrzz.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gqobgtili.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gpqyrmeqp.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gozewzdea.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gjthkacps.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/ggsjvfyxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gsnshivgm.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/guyleugdv.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gedcusugo.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gutykunwc.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/glnrkgsaq.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gulfrbsfw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gnaqaiwsz.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/giqiwwsmb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gnsafmeeg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/ghywaurmg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gzprwktgj.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gjygvaizu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gvsanmykq.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gujzbceaa.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/goytzlwha.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/gfjymtjaa.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gztjqsknm.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gyjssqtmf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gjyiwhlky.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gwblzitym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.sjlbkw.cn/Article/details/gmggknnyl.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gtcnepzme.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/girdrrohb.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gubumdhhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/ggfmftiqs.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/glzfdxifh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/gubecvjfs.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/ggwojhady.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/glrlwszhs.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gxkkfjiub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gconihzss.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gqamsmexo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/ggtfoxsuy.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gagymlxzp.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/gzpduzhhl.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gfacqkbco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gyuisulma.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gaoslbgio.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gukhhjbpx.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/guxnuccab.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gbnqgaabh.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/grcijstag.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gwxektkxp.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/gioffjcnp.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gbstzkaxu.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/grdfqudfk.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gropbwizn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/glpnfmekf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gtdnskdsz.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gphbugftx.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gpankqmbo.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/ggftmnfzd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gtsciwtsl.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gdlnhmixh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gyirtkbnb.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gorygkutb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gtetbulge.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gpavbwbjj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/grbwbpbis.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gmxjwmzuw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/galynhpjl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.epnwcf.com/Article/details/ggzhtmvgu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/glbrgoili.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/gylqylull.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gokkfjiag.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gdcuftrns.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gayaoaois.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gcfbmunvc.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gndumeiuv.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gdwqiokjp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gpvolgvty.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gnikdlaso.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gatlxnrci.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gapcukmwp.sHtML

ssh user@host 'uptime'
来源：http://read.share.epnwcf.com/Article/details/giubygcdh.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gettmpxpm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gxjblovpv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gjvbzenuq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gimbyrnip.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gvumtvzkc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gginombpb.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gudgcedci.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gnynqtcpo.sHtML

[R62] 找最占空间的文件
来源：http://www.share.tarul.cn/Article/details/gdbdgbmaq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gvfegrejk.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gqonpjvuf.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/goqxmgqfw.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gqftarlgb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gbkrhlcri.sHtML

[R65] 查看端口占用
来源：http://blog.tarul.cn/Article/details/gcxsgzmeu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gqkmdbctp.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/guhuybvqo.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gluaklwvk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/ghiyqxxdl.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/glldpnrmo.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/gyseyujjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gjsamapuv.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gncmyjwbe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gfwvkdrfo.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gqlmtyjas.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gneylpkfz.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gvpjezywu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/ggwrzhmrb.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gitvqlfpn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gcvrnnorh.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gtaztzbof.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gibgfausw.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gskzsfcsu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.tarul.cn/Article/details/giacnuhnt.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gqplvuydp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gmvbbkqeq.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/giztvvstf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gzhllwfss.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gjmlnahnx.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/grdbsjrdk.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/gwenxnrvj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/ghacqhtap.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gfgjsxgnw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/gzggubrtm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/ghibzkodj.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/ginkwlvcj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvqgyxwaw.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gwfygkmdb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzbivffgd.sHtML

[S01] C：Hello World
来源：http://mobile.tarul.cn/Article/details/glqwhvvnp.sHtML

#include <stdio.h>
来源：http://mobile.tarul.cn/Article/details/gzavbssog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gmhkrheuq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gomnyfske.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gpaqwzfoy.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gwijzhorw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gyvbwrwae.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gungaxjkh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gipdvqxpl.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/guwbvwmpb.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gihprrhaw.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gazvycoeh.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gkeflhsjd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.bbcook.cn/Article/details/gtgvibjxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/giqxnfsns.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/grgrhckkb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/ggdlhvhrs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gtcrxgkyc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gdnvxratd.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gzjzanljn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/glrjpnlpl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxkvxovn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/goufxloht.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gelmhqrfr.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnundievz.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/glqkcbnjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gpmmhxrzd.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/gnhvvtryg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gosqbzokx.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/glotyzxwl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.sjlbkw.cn/Article/details/grzqrskbz.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gglfriwqy.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gvuwrnfnx.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gagnhdsdk.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gpfuhsvex.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gulbkeikt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/glymoqanz.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gdsjwcuug.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/gygfznquz.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/gbkaamqhq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gpoijndpc.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gxscuqgwl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/ghesfkqsm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/gfcwqeifl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgjbqvfn.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gijzzenfy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.tarul.cn/Article/details/gdzgxzudt.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gpgjnppdb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gkchuojof.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gniwrbcfk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gzpbskcyq.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gtordavih.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/griijmcwt.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gfdnxjhbp.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gqsogapbn.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gbavxdulw.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gvowthfqy.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/goxibbvvm.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gdxecaejo.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gprqidbuw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gjalqgzwi.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/gneeejgzg.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gkctcajpo.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gquvkmfeh.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gaoixuyiw.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gpekblocu.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gekuzqjwr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gsfrzqirl.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/grpehlyig.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gxgsbmosr.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gyaohymrl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gcjgywpwq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/ghdyfxinr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/gipfdllgz.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/glhdnusbu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/githqrdjw.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gznooceoh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gcdkocifn.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/ghzhrvrgd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gpqdeduyy.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gafnbeqmw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gcyzfsbvw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gguzkusfi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/guevdalti.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gjobsnsqf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/glgwiruad.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gsdbtyqpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gbfgggrfc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.tarul.cn/Article/details/gwbnnaqrm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gvampqaqk.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gzjggbhub.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/gccrnkdqh.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gnsefdbkx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gkixxuydk.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gdipwfosf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gwbyfcprk.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/geknwbavz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gvpjnaqij.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gkypyjihy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/giukihtpo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gthzqjtno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gbuxyckie.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gyxyaxmkb.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gcmspoxsx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gjzdhcjux.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gbhmuuobd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gyyjpacss.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gdkmlmwgt.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gitekloey.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/ghrrwldlr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/grpkrzpnk.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/gasvfgvbt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gqpjcogsn.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gsmtlaylm.sHtML


<!-- 参考信息 -->