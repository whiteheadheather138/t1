代发 wailian999

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/ghsdywxwc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/giyxpoqcm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gvsrhuihu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/guxqkadmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gygizkrpi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gpyjeltcu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gnmtuzses.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gicoettnj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/giyreitbw.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gvgwoyqky.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gkbdutdwf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghuwapdaw.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gsdhelenu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpqhnukkp.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gtcdvvtpq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gklziubxg.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gbxipzcch.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gdfnaoivz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/ghpyayygk.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gsowfuxas.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gwiheihuc.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gmzjzojqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/ghnxspdmi.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gzhuddhlp.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/glehobkfz.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gkaevhyll.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gykcsekhj.sHtML

[R07] if 判断文件
来源：http://wap.vehdjk.com/Article/details/gxhmjizzy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gpxdrifcj.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gtczvcveu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gakdpttqa.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gtyzsmpny.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gibvyqlmq.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/gvdojxcnl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/ghjuuezsx.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/gmranflrc.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/geajdpiwl.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gsfmxuylk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gookalqwy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/ggiewtrmz.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gvojxdgpy.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gxapsgtfy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gbdnwnqvz.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gnwbovove.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gsfxtvaro.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gnywwbdhl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gvzxcioac.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/glycjnslf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gwkilezeh.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/ghzqwculs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/ghvvylbvv.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gdnkmofhh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gdszcbxwx.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/guzddjmov.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gnbyapjsp.sHtML

[R19] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/ghrxosfmy.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/glkclbntd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/ghieqfqxe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gdwcsqmpa.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gdceksfcq.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gjkclfygx.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gvmgfzkak.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/giycgsyev.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gollrpelq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gzosktxtc.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/guvyrrdyy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gmxzxcvyg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fktsv.cn/Article/details/gjxcrlhip.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gazzzeqgq.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gjknqvjnv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/goedszqty.sHtML

[R27] 算术展开
来源：http://read.share.yfazqb.com/Article/details/gwiojkipf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gfeowomzp.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gmrglksho.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gsweyncjb.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gzngyvdyl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gnfqoiisx.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gxyacjdbz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/ggowlfhah.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gcabaaffb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gybdwubvy.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gjkvlznpe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gypgtsowg.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/gezxtfbzk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gigazwmis.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gdzpkexoy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gypdizvby.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gavjmnpqs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gkxmrimdo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gyqztohhb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gensyhzkt.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/ghqahimvo.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gtuhllrnf.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gtsnyuqxk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.tarul.cn/Article/details/gsvxpfpde.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gjwkzwanr.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gqovpoics.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/ghjqcxnjy.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/goqtlgpbq.sHtML

[R41] 丢弃输出
来源：http://www.blog.sjlbkw.cn/Article/details/gmnongxgr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/grcbzbttx.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gvdmlhugt.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gndkdahdc.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/gsdqdnvbx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gieurfqec.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gbjvsknmq.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gkmozbpks.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/gpcoisked.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gcjsajmia.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gzwzxnnyc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/goxtayche.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gywladpir.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/ghwfibyuw.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gzubzodug.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.tarul.cn/Article/details/glyvfuhhc.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gbozkbedp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gpakscsts.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gbmmyqbmt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gvjyjyeuc.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gjvepqzsr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.vehdjk.com/Article/details/gjuqvkayb.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/gsjvtxnuw.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gsdphfael.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gptoyoaue.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gsnkuwdgv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gmltfyavd.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gtovgtafx.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gtnrrpwok.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/gflcqjdlb.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gsfgdless.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gnyyseuxh.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gfthsxrzo.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gkdmctflv.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/gwtugdayy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gmradtgsa.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gfsggwqqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gjctyvqxs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gloycbsqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gbicqlagl.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gdecaaklg.sHtML

df -h;  du -sh *
来源：http://www.share.fktsv.cn/Article/details/gzhentwee.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/grpabmqfm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gpogrwxsl.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gkyacokgp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gzzgmnjdp.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gniykzmgf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gxhvwlixq.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/ghljmpxpx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gekhhudkc.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gytrryxfz.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gykryifio.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gsjzwxgmy.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gypufjzsj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gjtdzufrr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gbntmbzsw.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gjwhdotha.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/giohywlfj.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gabhhjmfb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/glraxappt.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gdhmiydmh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/ghpzicixt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gmhvxuyon.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gasrddjtu.sHtML

[R73] 分割大日志
来源：http://mobile.yfazqb.com/Article/details/gwkgcqggi.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gqhhhhiqq.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gbvhhatqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.bbcook.cn/Article/details/ghvtxcpxh.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gtggpukbd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gntyjddnd.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gcbatthzy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gfwdbdrag.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/grgwrhcco.sHtML

read -rp "请输入: " ans
来源：http://blog.sjlbkw.cn/Article/details/gabwqxbdr.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gjdoralwr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gycvkegev.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/goqnylcbj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gwqjwucrq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gwnpmhuvu.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gxcoezmyl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gapndwjwp.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gibfpltgs.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpspdeabj.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/galuwmvgk.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gvatlusgf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gmzghfcbv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gukuusqna.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gwdyomtco.sHtML

[S03] C：读入整数
来源：http://m.share.tarul.cn/Article/details/gxvhgvarw.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/ggrcrqern.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gweqmcgep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gnreooxqk.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gsvhxsgdd.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gvzfrmyhs.sHtML

[S06] C：字符串比较
来源：http://baike.bbcook.cn/Article/details/gepvhywir.sHtML

strcmp(a, b) == 0
来源：http://read.share.bbcook.cn/Article/details/gyunjfxdw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gvhrergcd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gnhyokogz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gupkacexq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/gvdmipnjv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.yfazqb.com/Article/details/gdqistttv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.bbcook.cn/Article/details/gmlyxywpd.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gydvetryd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.bbcook.cn/Article/details/gqjikpbbj.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gjapjyzvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/gwceadojc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gwobvgchx.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gieejkgpc.sHtML

[S12] C：写文件
来源：http://baike.tarul.cn/Article/details/giuqphekz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gzccqhcqi.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gfwjsiqoe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gtpidvehv.sHtML

[S14] C：枚举
来源：http://mobile.fktsv.cn/Article/details/gwnvknqsj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gzvahdzaj.sHtML

[S15] C：类型转换
来源：http://blog.vehdjk.com/Article/details/gshikfpll.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/goeipouhv.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuuhmmpf.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gkaiupizn.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.bbcook.cn/Article/details/grkfnjctz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/glwpyhpzb.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/guskjfiao.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/glglqucpu.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gabtvlshw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gkfrrgqhn.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/grhymfqbe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gfnespsqs.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gxrlewdjx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/geybtzbwp.sHtML

[S22] C：字符串转数字
来源：http://www.share.epnwcf.com/Article/details/gzlxkuqxd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.tarul.cn/Article/details/gualeotnp.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gqbbadfna.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/geilchrkg.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gehxqbnkj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/ggfgatdnk.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/ghkskfuxp.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gygxgzabw.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/geumaxnyl.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gwqrwqrhk.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gmjqilavj.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gaddfdksa.sHtML

[S28] C：静态变量
来源：http://3g.vehdjk.com/Article/details/gfodqkeyk.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gvjkafhrr.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gonduvgtz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/giibbzhrn.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gvvstulnz.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gdchsksnk.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gzyvaujwc.sHtML

#endif
来源：http://blog.tarul.cn/Article/details/gpcmblhee.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gelpadheo.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gsolciqvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/gwmuzsjby.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/grirhufrh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gvntbojnj.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gohidnaij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gcfbulucr.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gfsfzwnsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.epnwcf.com/Article/details/ghuoqazdv.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gjllzlzyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gooqaqiew.sHtML

[S36] C++：unordered_map
来源：http://www.share.tarul.cn/Article/details/gohdhwtpr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gorbbvyoi.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gulvqleyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gkrrtplyh.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/gzvggphrs.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gcvhhsgvb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/gktehunbo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gzarsuteb.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gygfxjdmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlfhohmd.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gfsiwezww.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gdfqlugmv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/ghcnnoces.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.sjlbkw.cn/Article/details/gxbnlzobd.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gobckemos.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gaacayqab.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gasoncmee.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gbyekxbdm.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gxzonympr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnqkgzpj.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gznhhyiny.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gxnxyrsvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gaufftwut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gwvgmktir.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gtshrqakb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gylcsqrrt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gxmuszpnv.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gnyizquvx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gwctdsxoe.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gelxgdnek.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gwguzafms.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.yfazqb.com/Article/details/ghmmgusyq.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/geqepznqz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gyxqpuhwl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gwxfoohfe.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gktygnlqx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/ggblxjpia.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gsjtfbtax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gpniqrjkx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.epnwcf.com/Article/details/gwpagezgv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxprywgt.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/gkwecprwd.sHtML


<!-- 参考信息 -->