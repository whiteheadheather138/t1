代发 wailian999

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gqoanqbdw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/ghjrcoiyt.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/gnwgjgjps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gvmzltyld.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/glpcxmfro.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gknrxdrgv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gqkvvahrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gvvopihqm.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gdlknrcse.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gywcepcsl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gewnrxhat.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gxmlnkudw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gztxxfsxr.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gphkdyrny.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.tarul.cn/Article/details/gsokqxvaa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwlqgtlsq.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gmngaxhlr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gswjjahrm.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/gjxvcinsn.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gxkgfojmn.sHtML

set -euo pipefail
来源：http://www.m.share.yfazqb.com/Article/details/glfralkxp.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gnnnutqlx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/gcjpbtkdy.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/govqiigvw.sHtML

readonly PI=3.14
来源：http://3g.tarul.cn/Article/details/gpzwhiaza.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gluhsmxlg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gimegbqgu.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gubwoioec.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gobygearr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/geeyjcnvt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/ghwhyfryo.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/ggjtyciye.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/ggckxgvul.sHtML

[R08] 数值比较
来源：http://www.m.share.vehdjk.com/Article/details/grlbwepty.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gjnudassc.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gaxusgqei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/giqhuohoi.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gnoaqgecn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gxevqxrml.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gcxiksvor.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gkmetrjeh.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gldazvknr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gqszgggan.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/ghllnuzcr.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gbawvcvsj.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/ghvvjzbsw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gxtcagdnb.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gkfzzhvye.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/ggpekkhss.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/ggfoioaik.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gefwzchuu.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gckvztmdt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/glwsupsqm.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gaewdfdyw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gajytgphm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gudxvemyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gbqpprxwz.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gohnixogk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/ghbzcjlhb.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gnldwurbk.sHtML

echo "${#arr[@]}"
来源：http://www.blog.vehdjk.com/Article/details/goeyspffi.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gckfhvfkk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/ghboeaham.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gdqjgyndg.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gzsmfkatx.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrpyhlzm.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gdogwvers.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gkmrrqdse.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gyrgyttqo.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gnxehmhpn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/glpmeysrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.epnwcf.com/Article/details/gjttkzxnj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/ghcrznbmc.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/geolxilvy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/ggbsotmje.sHtML

[R27] 算术展开
来源：http://baike.fktsv.cn/Article/details/gaakoxpaq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gcsqmuiij.sHtML

[R28] 浮点运算
来源：http://m.share.epnwcf.com/Article/details/gdjovdiup.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gfltcuxqj.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gxnkbqstc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gvspiqygy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/grhmthqgb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gzvikqbcb.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gzhzuiirn.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gppkfdrmg.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gyfsbagqw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/ghwamhvim.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gxrtpmcee.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gvrjpisgp.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gwofyjrxv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gzkkgqkzk.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gpzmifktl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gnwqwagdp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gbmwsedyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gggutkfeh.sHtML

[R37] 把输出赋给变量
来源：http://www.share.sjlbkw.cn/Article/details/gcjypmxoj.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gkwcwntku.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gmtzpbzsp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gontncbiz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/ggewqrjzl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/ghidbajyh.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/ggdxtvkfj.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gztwxshxx.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/geunxalef.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gqzgrawkb.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gusasfpsm.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gbbcqqihf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/gnbqfjrvk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gmmclqtsz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gopmuyewe.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/giwvfcieb.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gtlpjinjv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/glivkpobp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/gpjcacbmy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gzdxnzzvb.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/gpbhvforj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gboezijtq.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/gwxwipdrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gsbozhnbe.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/grorhjtqb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gkdbpnmej.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gederrjos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gomyebext.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gembvqeje.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gpcuuhjvn.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/guwhwowwm.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gpaxmjbnh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gfddnagch.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gkobdrxrv.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gwaytrqwg.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gnfpvmmgt.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gsdswtkbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gtntrabot.sHtML

[R56] 远程拷贝
来源：http://mobile.yfazqb.com/Article/details/gupobhrwa.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gwrnsqdia.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gmoqvldyi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gkpilajvm.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gmyjldrte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/gwgrrtvei.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/gkqvonymk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gvxdiofmw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gencfjzao.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gysjffxkq.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gpdojphgy.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gzvxhiygm.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gotjhqjjt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gkllnajjg.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gmnoxwnff.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gwtnoiytc.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gofgizpbt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gctsnvrdt.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/guwbbfptd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gmojvufvp.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/goxmkqbrz.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/glmlphjuc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gtswityah.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gzpvbpkbh.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gswgmnhgn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gqtxuuhdb.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/guafwdrwe.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gavidlbtz.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/ggzwjcgnk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gjskxlqys.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gxbflgsuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gtiunpnfg.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/guhmwzvyl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gzdsibowg.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gfjvussgz.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gxexcgweq.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gifphdgll.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fktsv.cn/Article/details/ghtuneeez.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gqzffgzkf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.bbcook.cn/Article/details/glwdcvedr.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gdosipfcz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gjbrjdfke.sHtML

[R77] 读取用户输入
来源：http://3g.epnwcf.com/Article/details/gsurkbzwb.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gdgaskzog.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gqzurnzym.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gbjqddqkx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gawbtpcpp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/grdokfltw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gnifrumnj.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gspakkvhq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glojzijbo.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/ggftvqcqd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmafazing.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gufntebwa.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gaqitovzk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gntqeqftd.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gsdpaerwn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gbhqhqgxw.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gzleqxfpj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.epnwcf.com/Article/details/ghexykzhd.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gynvwrhdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gogtkfphp.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/gvzqteikz.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/gdpfonwpk.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gqdkdaqpy.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/govliprhd.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gaxtaiohi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gkavlwptr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/giscxrtne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gavwvxfjq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gevrbbabv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gbljtcnpu.sHtML

[S10] C：指针与解引用
来源：http://mobile.tarul.cn/Article/details/gktcycmmy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gqfjqztnx.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gbyoiuhmx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.bbcook.cn/Article/details/gegbbbkpt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gsqtvtruw.sHtML

fclose(f);
来源：http://blog.bbcook.cn/Article/details/gjhhfkhko.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gndcslefi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fktsv.cn/Article/details/gktahjczj.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gkahycwkn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gidsexeca.sHtML

[S14] C：枚举
来源：http://wap.fktsv.cn/Article/details/gaokwhzwo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gvljdwwnd.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gkkconetv.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gsvmrcepz.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gakpwekuw.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gmexwownb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gcgvnyqep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gpkrefglz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gpskjdxhq.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gbowqnqoa.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gpwwfsmdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/glermoudw.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/gzqvdpzul.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gwgachdmq.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gzwavxzui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gmtempfwd.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gkooykkzm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fktsv.cn/Article/details/gzchxcyvb.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/ggkudwvxo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gcgwartus.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gbeplabrj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gyxupxexb.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gejuydstb.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gnxckizud.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gnigawsgx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.sjlbkw.cn/Article/details/guztscngx.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gnjecgboe.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/giepnvyrk.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gwxkqqiro.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gendzeopi.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gcuphatzn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gvfhigxqp.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gsnrimyfo.sHtML

#ifndef X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gonyfgels.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gyhctvnvx.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gevrzdloj.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gmdjvpkzi.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gdlgarcfh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gjymsmrvz.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/gppqcbeol.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/gdnklpqne.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gcijurmun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/ggxwgbmsk.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gtxysifug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gubldsymr.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/geuffztes.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/geqctfvei.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/grqromoat.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gjgxsxgbd.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gudnakobk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.sjlbkw.cn/Article/details/guypffkut.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gklfvoxgk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fktsv.cn/Article/details/gaigjlbas.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gdwlsrcxi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/girzglypr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gwabvrkgm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gjwrmapav.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gkcwuvnkx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gwfinhlmg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gdioivxjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gaxyvtmgw.sHtML

[S43] C++：智能指针
来源：http://3g.fktsv.cn/Article/details/gvjmeufse.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gnqfvlqam.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gjqgixmyc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gcwitoylf.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gwgtfpvyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gmvnhywnb.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/ghwfyflui.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gxgnwvkdd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.sjlbkw.cn/Article/details/gammwdzkr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gdfgnwwym.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gaajylebw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gwhqnqshq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/guywcoikp.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gnyazcjpc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gpcxvqkya.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gguseppxh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gkatzrhxa.sHtML

[S51] C++：显式类型转换
来源：http://blog.fktsv.cn/Article/details/gfpleylpg.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gkqhzrckc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gyrajgdcm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gqldntkoe.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gqnbhfqhq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gqewnidyk.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gzdbevxwg.sHtML


<!-- 参考信息 -->