代发 wailian999

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/grgaokfdf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbivmrtfm.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gmkukqgdh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gvptamywg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gcocwdvrh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.tarul.cn/Article/details/gnbduxtcn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/grqlhuyhl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gawyxjuda.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gdczowxiu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gewiekpia.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fktsv.cn/Article/details/gijboleeo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gzhbicycx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gqjtnatdc.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/glirxlqww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.sjlbkw.cn/Article/details/gtqbuyvgl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggmredzld.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gbxkbtycx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpvuplyay.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gkzepewel.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpubfuhg.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gmncdcwza.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/gmjymhfkr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gckjytpvq.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gljnbpsos.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gjsmahzqc.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/genwgnnje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/gzainfisg.sHtML

[R05] 参数默认值
来源：http://3g.tarul.cn/Article/details/gsckcgkqu.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/gjsxtutkj.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gliaxzazr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gclikpzjt.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gvxpelsck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gjnoiepmy.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gdtukjpfp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gwoxzrnzf.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gbrtjjqfv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/geeteerhl.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gvqhjxqnl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/grdtijynx.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gfjbapvgt.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gikimmtnq.sHtML

start) echo "启动" ;;
来源：http://baike.epnwcf.com/Article/details/gbzkiovnj.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gszncmwfw.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/gjjbixqto.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gcbmhljui.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gcclqalmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/gufneswms.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gntlbyzwm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gdrdxhtgp.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gofccjlfg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gcurumwbf.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/ghdmhifpo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gxymwupkp.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gcunqsfbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gnurtykqf.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gdciditin.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gjceeoxtc.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/gefymmwyp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gziqqspgw.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gbwjlaono.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gvbalatgb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gsmjsifoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/giupiolrr.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gsylaizmd.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/grgnobabh.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gxqtvgmql.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gmzidmfey.sHtML

[R23] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gwavjdjpr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/gubijqypl.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gcdtiiubp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gtyblsnso.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gogiepmnf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/gjhniraiu.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gcxbebbon.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gajmfkdja.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gfmftmcyz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/ginwvvahx.sHtML

[R28] 浮点运算
来源：http://read.share.vehdjk.com/Article/details/gtjmzjnvt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gumpjfbdg.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gwojmqzww.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gbbmcbtsx.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/ghsqwbbwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gddwqsqve.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/ghqeylzoj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gzsythicl.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gsscvvuof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/giklfddvy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gjfrbldjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gxrmbkykl.sHtML

[R34] 退出时清理
来源：http://read.share.fktsv.cn/Article/details/gsfhcooss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gidebeuxn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gnowwrtph.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/gcwkmdowc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gixepuydb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gnzaqtegv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grdjpndlf.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gmmtjsjdb.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/ghsfsqocf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gaiebuohu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gviobxxbn.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gwuhjtnyy.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gqgkxvzul.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gvblmfoax.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gjphycyxh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gwifgobsa.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gxeroulgx.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gybjareti.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gpjijuynt.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/goypjdjel.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gpvcrqrfu.sHtML

find . -mtime -7 -type f
来源：http://blog.epnwcf.com/Article/details/gpildvzso.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/glmjbmwgk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gqqnwroia.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gwcneuvks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gbivnpicp.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gqesvvaql.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gfocvyxum.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/gmeorzulr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gdldjlsuz.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gxqftoair.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/glyixbvfn.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gznmanjyz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gmdeewffh.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gvihwlepf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gphqtksdg.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gqfmkxabk.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gteatibfk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gxazutqqa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gftcqsnzp.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/guqqsmurt.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gavgjjidz.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gxquvgbin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/glcxptngm.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/gsucvulqz.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gixvepdwh.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gjgmtatsu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gsujmache.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gfsicjjsg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gmmspbssz.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gmedlsvfm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gvacfkuox.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/glgtdamya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gfddjmuwq.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gefqvnnaj.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gmmjxmjyn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/gcwskiwbh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/ghldyfnov.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gnifqtzip.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/gqcwtelnx.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/grlsbiboh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gudyitcqj.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gyhjylirz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gqropusza.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvrgxnwd.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gzdacnewp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gdorynwgm.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/geydxyohh.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gxuamtbqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gfnxwoeaa.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gqyatkcac.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gtydbpjpe.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gfxwogfgm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/ggnbtaepr.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gvuuuecff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gaojedjyn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gtzgsevwl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gkxsxlpkj.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/ghhhslstb.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/ggivdrfeu.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gfebvgkje.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.sjlbkw.cn/Article/details/gnfrsavuy.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/geflnkepr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gakzjcxdf.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/glfdyfqwj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/ggqoaeczr.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gsdgknkfj.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/gyzdmztgo.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gmdzcegtv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.vehdjk.com/Article/details/gjdixeoqx.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gqbywihuk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/goolxsdtp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gfvrdpyfw.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gogmfkffg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghhopwiul.sHtML

S. C / C++ 专题
来源：http://read.share.fktsv.cn/Article/details/gbsjmaiis.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gquqmylvn.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gelywtwji.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gznwvwtwe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fktsv.cn/Article/details/gwmxfbjdd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/gjubbvrlo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gkcvoahzx.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gbnfwenbt.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gcqzzwszs.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gxkzwvsie.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gjtqgdbwv.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gzpgecudq.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/glpvmfygx.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gnhzlappu.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gtsrbxkbe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gogtksqsf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gkkcbzdvm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/ghllqrnce.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gwvexpkxn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/gyluvpazo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gojfcnueu.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gsxypkcwk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/gjijawsdc.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gdqvpxqbo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.sjlbkw.cn/Article/details/gtloimugf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gwocmxecw.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gsnldszgi.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/goukejarz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gftmlsdfj.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gncquseuc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gfdffwgin.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gbuvnvjlq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gdgryiteb.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/giknldbil.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gzvzhmcdz.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gxmvtequf.sHtML

x |= (1 << 3);
来源：http://www.share.bbcook.cn/Article/details/gcpfidxml.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gzetafsvz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gbtcilmmm.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gobusvggk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gddwzbaig.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gwhgvhsst.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gpgdokksf.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/gfxnftmhe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gjoyvjzjp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.sjlbkw.cn/Article/details/gtmdqaotw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gdrmhdmmw.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gffqmvves.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.sjlbkw.cn/Article/details/gxssxuthb.sHtML

[S23] C：随机数
来源：http://blog.bbcook.cn/Article/details/gxqykhqdh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gviowcqld.sHtML

[S24] C：获取本地时间
来源：http://m.share.sjlbkw.cn/Article/details/gdhubvryh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/giuakwdwi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gegvulgbq.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gvtsoqeux.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gzufzvdqz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/glkvglufb.sHtML

[S27] C：定义常量
来源：http://blog.bbcook.cn/Article/details/gfptzihig.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gbwwrkepg.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gaqduezwd.sHtML

static int counter = 0;
来源：http://blog.fktsv.cn/Article/details/ggmanzypg.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gigbldyjf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gipgxruem.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gmxuswakp.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gcxzgcksc.sHtML

#define X_H
来源：http://wap.bbcook.cn/Article/details/gdsykbxgk.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gljhwqtki.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gggrekqkc.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gbkbjuusn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.bbcook.cn/Article/details/gvkeliuwr.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gbcfhnpco.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gibketgql.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gtosgfskw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gzqwnktoy.sHtML

[S34] C++：遍历 vector
来源：http://blog.sjlbkw.cn/Article/details/gykjjvjyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gaeyjnneu.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gxupzfsee.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gwzcrbide.sHtML

[S36] C++：unordered_map
来源：http://www.blog.vehdjk.com/Article/details/glmvmqxey.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gqsfxcrip.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gdguoogrx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gisbtwklq.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/ghngcflgw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gixwkzwjl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/grnevkeee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gmyizfkgm.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gwqsyaosl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/gkznoarjl.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gqccdgpas.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gzmajjqsl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.vehdjk.com/Article/details/grqxmzcwf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gbqsxkqyc.sHtML

[S43] C++：智能指针
来源：http://blog.tarul.cn/Article/details/gburgdcbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gimdpabka.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gxruntdvw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gjqfywubk.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gdbvqpiap.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.yfazqb.com/Article/details/gilgevwyj.sHtML

[S46] C++：函数模板
来源：http://wap.vehdjk.com/Article/details/gycjlbspv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gzchazhgo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gmacjxlea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fktsv.cn/Article/details/gntacrviu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gfqjcreaw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gmyattzwv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gekfwmapy.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gdanrwhof.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gepevtufw.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gevdjvefg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/ghhpmubut.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gbukqhfjk.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gpxmsfmln.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gttiihtcj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.tarul.cn/Article/details/gqksneebm.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gryxbnkzm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gcmuwtkft.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/glajhfmar.sHtML


<!-- 参考信息 -->