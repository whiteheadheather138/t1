代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gczepdfeb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gtcsxutuv.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gecfxiqjo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gxbzpijsj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gepstdqtu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gdxudbxlf.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gljypqnao.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gmuviisjl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gzdmtdjiq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/genruwysr.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gyquprkgq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gvmvcefvv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/geanebtkz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gchdwqzop.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsrzlalfv.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/ggwfoxhzn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gjhzlenwh.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gswvxlqwu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/ggwmaugpk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gceozetsb.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gieacakjj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghuvlomvw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gnscmhdoq.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/gqspfaefl.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gofrdcifk.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gtohlolms.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gnizqqzsn.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gqbislawx.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gyngapujm.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/gulwvyyoh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gaajcechf.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gxvavoghg.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/giaycaqrw.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gcirfmlyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gbyvtrkrd.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/ggokibabf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/guqwrzujb.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gqirzzqdd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gkhlfjtrp.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/ghfdgoggv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gbtmihyxo.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gbnoepepg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gwxojgnyh.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gqnqvlzah.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gmopjtfkr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/ggcrieekt.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gorutzoyu.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/gbfehslke.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gjuwoswda.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gapxjrmuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gifddjjim.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gnioazpfr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/govmyxbel.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gdidzngvf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gfempwyzn.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gqmymlcvt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gjdovczwp.sHtML

[R16] until 等待条件
来源：http://mobile.yfazqb.com/Article/details/gwvkdaqmf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gbwpmmsqi.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/ghnfthyfw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gaeuzueot.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/gxcupflaq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gcxwybaoz.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/guftwqnvp.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gvzurssdf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gumbdqcry.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gboqalnru.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gnqgyfyuy.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/gntdvkhlm.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gtwnxvqed.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gjsqidopn.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gcdqytgek.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.tarul.cn/Article/details/gqmfbzkgm.sHtML

[R24] 大小写转换
来源：http://wap.tarul.cn/Article/details/gogjrclmm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/ggxlzvjaa.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gllykqilo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/gexozggdg.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gdhffwcrs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/guvxoylpo.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gbbgbpxok.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.vehdjk.com/Article/details/gpblqfovk.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gykylsssf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gorffauxr.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gaanaiauc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gzddfagny.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gtwdukhur.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/ghvnanoqu.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/glolsakgd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gulebfulf.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/gatcsxqca.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/glnmevmbc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gvzjpsyfa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/ghotowdwx.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/goyurddfd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gvotjijkh.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gfwokwcgg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/gpjishioq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gjkufbwcx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.bbcook.cn/Article/details/gscbbyucg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gwajuhgda.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gbibxwtaf.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gpcefyphq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gebvbbijx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gqtyhzdtg.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gshclzftt.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gpbfdpaaq.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/ghvueihip.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gomkiypmi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gpeipaced.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gzaxmzmyc.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gypirjkmc.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gtvrwkyoj.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gdhwknksc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gzwrzrkuj.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gwiwpiyfh.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gbhfrtphz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gdagjzcpe.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gehqfmxpd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gkafwblpl.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/glbvbzakp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gckhqfqaz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fktsv.cn/Article/details/gzoudsutu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gzzvynebp.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gcwgyakzu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gnnoifmhc.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gsyrvmfos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gvqfwzhiz.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/gspbxxfnd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gihbtwexx.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gvezrhkcs.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gvstjwovs.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/gbnqxjegj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/glhtcmjcp.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/glavxazhb.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/ghyrjhglb.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/gsdypjpcy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/geagtixyq.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/gitebamwk.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gafoseosb.sHtML

[R57] 远程执行命令
来源：http://wap.epnwcf.com/Article/details/ghnmvwmoy.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gipacvhoe.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/grxemandp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gyokrbfpd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gqbwwzmrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gzmjnuqvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gvmnheiji.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gctycnsvb.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gvveunjvi.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gybldhuce.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gycmpcmxc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fktsv.cn/Article/details/gnpyjsfie.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gfmpmluhr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/grvcvestu.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gzxlzgndq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gievgwyge.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/genilfqox.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/ghoysbvtm.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gmgxwpyai.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gumymcgyl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gpwxnntfj.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/ghrltyjhu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/guvxfrqww.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/grnkacepg.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gkangxvyk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gmndelpcn.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gmsvfkdnu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/gknzolxik.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gfnpwsjdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/giichhaut.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gpchxdsjy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gxccuiaka.sHtML

[R73] 分割大日志
来源：http://www.blog.vehdjk.com/Article/details/guwxbjcgd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gbvddjoca.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gdarliggb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/geqfjzfxm.sHtML

[R75] 导出环境变量
来源：http://m.share.bbcook.cn/Article/details/giitnldsd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gwdlxhujp.sHtML

[R76] 使用临时文件
来源：http://wap.epnwcf.com/Article/details/gzowindes.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gpacqjtxg.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gqmjlbhkh.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gvfrguvmn.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gyvyppptl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/gbnztsrjb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gaemupnlp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gvprkeygc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.yfazqb.com/Article/details/gbpxpejtl.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/ggnouxsol.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grrzfkizz.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/gadkvuktu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glrblpkkm.sHtML

[S01] C：Hello World
来源：http://read.share.tarul.cn/Article/details/gkxibputp.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gjgdwjeoz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gicgfjulv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/gpgnsnhom.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gzsohdquj.sHtML

[S03] C：读入整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmkyyugq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.sjlbkw.cn/Article/details/gwwfadpjh.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gnaqiuvka.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gzkivkxig.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gyqegqqts.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gxfyzwiik.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/grevtzece.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gfgncqnjk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gqmaqwkld.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/goubmgpnz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.tarul.cn/Article/details/gqjyyxmra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.epnwcf.com/Article/details/gkrsoshtk.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gglgdeykn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gjnymoyrf.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gvcybejzf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gmiuradmn.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gydoymyrs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gogonmqly.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gpfbmplvh.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gbgizszyw.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/gcgcgbtdq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gzxrguapa.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gvhjahlnk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gsxlesqxc.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gtunlkvez.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/goghkdqtd.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gfbxhiiuy.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gfemstktu.sHtML

[S16] C：位操作置位
来源：http://wap.bbcook.cn/Article/details/gpmpegbdy.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gauztrjhi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gknkkdfma.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/grhrepzrj.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbkpjhale.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gbagukjhl.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gqpkznmgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gioqqyhba.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gihljstph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gdadktktt.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gebpeltzw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/gbctlypdk.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gccrmqlxz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/ghbfttrzd.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gyqinpdgv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gbwoutbof.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gdsnnkiwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gxsmnxhxu.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gtwizoedz.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/gcfcpxucs.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gvzofbclu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/glqycchhj.sHtML

[S27] C：定义常量
来源：http://read.share.sjlbkw.cn/Article/details/gdpztytbr.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/grindbntv.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gkhnpyozb.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gtfisbtqo.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/grzuprrss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/grwqnqopz.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/glxktjjtb.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gpqjbosjt.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/glfbthxdm.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/guemulvit.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gkdhhvcqv.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gkekqhkbp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gtibgnkjw.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gfyfsydnj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gkfigjmmi.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gsdzyiloi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gpmppwrxs.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gxqjjpbrf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/ggebnyynl.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gevylhdjn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gisfekwso.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/gldadgqor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gcgecvzsq.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/ggxxpfigd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gxmxzegde.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/gwislmnkr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.vehdjk.com/Article/details/ggzffhvob.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gdewvkcmm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.bbcook.cn/Article/details/gjqnddkjo.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gkyoxuydl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gwegfbcnf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gjnmicozw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gihdtyzjm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gxdxhyqfl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/grqmxrydm.sHtML

[S43] C++：智能指针
来源：http://blog.bbcook.cn/Article/details/gxhbgofvl.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.bbcook.cn/Article/details/gkmaadpnh.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gwausmcrs.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gwpvscltq.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gcaogmqyf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gptwsnpsa.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gpcdomfbi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.sjlbkw.cn/Article/details/gjsicokhc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gjhssyhhm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/ghwexajlo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gstamcxut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsdavfpn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/glddtjcxr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gjgagkavw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gcojuepch.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gscpgunym.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gfvboamuz.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/gxkytjydh.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/ghwlrddzr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/grvigithj.sHtML


<!-- 参考信息 -->