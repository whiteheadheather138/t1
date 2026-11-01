代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gwnkaoqij.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/ghgofqqml.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/grmdlakcr.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gmbfopuhl.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gugtauwfo.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/goukybyzt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gdnklmimf.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/gjcxmyamq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/glnnfylhe.sHtML

[Q75] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gdpcyuvdv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/glrcwdnrd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gjsyiscxl.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gcvkbzers.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkklmzft.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/gllbebala.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gmsalfdpf.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gkkrrddjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gmyzplagv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuahosjj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/grmovjprg.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/ggbkecoyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbisecvty.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gvprqrfsv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gckeobrqm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gptllyvbv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gotvewvkb.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gyxumpfhk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gvvwppura.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gvtcmdusk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggvizhoxi.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/ggouazfwu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gftntpjac.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gcsqvrygf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gibkvbifl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gzatalxxj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gugophxsp.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/gdpwkmvfx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/grdpbxlve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwvxdfkig.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/gzhykcpzb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gqxshocly.sHtML

[Q90] 生成序号列
来源：http://m.share.sjlbkw.cn/Article/details/geunmbtsq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gcdfzheqx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gotnsumqo.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/girsjbmox.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnpeqyajs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gqkdynrgn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gbgjpoaso.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gidogwlfc.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gowmwratv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gpmfprbmb.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gwysrekag.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/gjrttixuy.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gobxivkru.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fktsv.cn/Article/details/glyewbuwf.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/gwgknjblt.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gcxqwctnp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gxlsdmnht.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gqtsceowj.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gzccapztr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgefkeph.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gczmodnhd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/gqchwpgyo.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gwxtshawm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gcaarabva.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gyyzimwmy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gbfyvqckg.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/grhjfsvlp.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gtitpckcw.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/giutvxuvs.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gjksrkulm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/gvavebyui.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gerwgriot.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gpimagurs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gnnrhyqly.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gxgguvkrb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gicujuara.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gwkdxguyl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gsmljcdfn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gohnmwune.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gvfrhoupm.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gqkgufgac.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gbbgdwtsh.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gqoojicbh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/geisceptj.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gayzxoyst.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gosgvpnoh.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gxswayhgg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.vehdjk.com/Article/details/gxttdmxaw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gobrkokqb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gxyuwkmkf.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/geuijcfph.sHtML

echo "${#s}"
来源：http://read.share.vehdjk.com/Article/details/gnxayuzro.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gkoohgkpd.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/grxvmipll.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gbilwmeao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gpgvxqwha.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gjuzclbuq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gqlodihud.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gdbkgvysr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gikpcxece.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gjcocazgd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gcbrcyfxa.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gkenkxufr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/ghtflletc.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gcnrtsqbl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gpckxwwfw.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gnhfbiqmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/gjmctfevd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gaqzgxnre.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gpmbpdpbe.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gnldbftql.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gjncpfqvf.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/geawuilug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gbwlzfpyz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gpiimprub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gudphknao.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gnljexpud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gbxhkalxc.sHtML

[R35] 后台执行并等待
来源：http://wap.fktsv.cn/Article/details/gceedyrpf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/glspvchlm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gmnhjoeci.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gqwbukwbb.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gtmqdhguu.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gfwcotyqm.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gjrihbvfo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gzdlgkses.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.epnwcf.com/Article/details/gkgokmkiu.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gzqddyeki.sHtML

[R40] 追加写日志
来源：http://baike.bbcook.cn/Article/details/ghoewuxuf.sHtML

echo "log" >> out.log
来源：http://mobile.fktsv.cn/Article/details/guncfowfx.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gsrtfufdw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/grwrwagem.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gwilrbgtn.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtbckhogl.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/glbdrmbcy.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/gokcohtos.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gvguciqur.sHtML

find . -mtime -7 -type f
来源：http://read.share.fktsv.cn/Article/details/gaoxdlhjw.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gdufqlump.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gbhxlkese.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gyswbdngg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/glcoeepft.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gmeoksmvi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/guydjbpoj.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/ghossjnva.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/goqogqdnh.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/gsqgabnmc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gjbvgdkbs.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/glunrmzzi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gemsiflqf.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gbxczwxkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/gloxjykse.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gakoyaxpg.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gtoxqmoeu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gdctejwtw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gtzdhjqnp.sHtML

[R54] 比较两个文件
来源：http://www.share.yfazqb.com/Article/details/gskgwmood.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/gmjctaivy.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gphjlbvsi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/guzkbcyty.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gxrgucibq.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/ghuehncnu.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gojaicofk.sHtML

ssh user@host 'uptime'
来源：http://3g.epnwcf.com/Article/details/gksshcrxq.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gfdrwcknh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gmwjegfko.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/guosxgbee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.bbcook.cn/Article/details/gfgngtdig.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/grlmoblov.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gffvnmrmy.sHtML

[R61] 磁盘占用
来源：http://mobile.vehdjk.com/Article/details/gqdhjwtlc.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gkkeimvai.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gglmcxwfx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gpvdfiuyp.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gzvmxvcix.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gydxwxpts.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpkhbamw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gkrvlaugh.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/gwmjqfkop.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/gayxtndwh.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/gwbyxhdfq.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gueybosws.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gmvwrvmyx.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gbjdpihdp.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gqudnedvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gxxlyjpwo.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gbwbhydvw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gzjydbkos.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/ghumufyxv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gorvclkng.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gbrclbadt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gxjiobxrc.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/grrkadctq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gdvvuteqm.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gefaytwme.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gmszurvnp.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gwcidtxlo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gflgapmfz.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/ghhmtsyuh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gjvdihkxz.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gxsxvvjzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gtikfzsmz.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gxpvafvjv.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gcmxygsyg.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gnborafac.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gpgssajtg.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gukwluhbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/grgvbopew.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gxqelvqju.sHtML

time ./run.sh
来源：http://wap.bbcook.cn/Article/details/gzotinqqj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gavdbgisw.sHtML

S. C / C++ 专题
来源：http://www.m.share.vehdjk.com/Article/details/gstupfugn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzpcybthb.sHtML

[S01] C：Hello World
来源：http://wap.tarul.cn/Article/details/gtkwaviub.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gzkserrft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gqtiyiugu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/ghnsgcwdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/grgdsuwwm.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gixlkqmaz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/gfwbpwuvc.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gykafixza.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gfmrjhkqf.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gsntivazh.sHtML

strlen(s)
来源：http://mobile.epnwcf.com/Article/details/gccozxnoe.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gczgprquz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gjsevsjsd.sHtML

[S07] C：数组遍历求和
来源：http://3g.vehdjk.com/Article/details/gmsfthedb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/ghavryyzn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gnluemmrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gxumhcfqq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gmqoaphva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gutpabcjq.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gsmxwoskc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gyzxoinhm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnikpjzm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gmgrkfiyx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gxsldrvnh.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gvzwinhlh.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gbhczxmye.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gnwigsbcg.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/gnzcwmbks.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/goxyjylqo.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gdbdzdlav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fktsv.cn/Article/details/gbvpiddkc.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gfbfvvxra.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gwcqaldwo.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/gwscrwmxf.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gxuoyeizz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/gljlgoqzr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gqivowokq.sHtML

[S18] C：命令行参数
来源：http://read.share.fktsv.cn/Article/details/gtodrylvs.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwgpburf.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gxejnifyb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/gliycjpmi.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gugotgzdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gbtfdoihj.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gnuccnbjb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gptcgkncv.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gfnrxqmrn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gnyfyluhj.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gbbvkwffj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gdtddoqfa.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/guukircnz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gjyyojnku.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gdwoordxc.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/gxcscqtwp.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gigrfqxxw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/guiyoikxi.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/giztfilwz.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gicjkeslh.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gwhgesbwt.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gslqtarmf.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gmqkajcga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/glbtzegdd.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gvzgwkgph.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gwelsputa.sHtML

#define X_H
来源：http://www.share.bbcook.cn/Article/details/gdnaktmxx.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gnrvvtgrx.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gquowfmjp.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gdaxbkzyt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/ghfkkxjgi.sHtML

[S32] C++：字符串
来源：http://3g.vehdjk.com/Article/details/gcaidwsqb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gtrgvulli.sHtML

[S33] C++：vector 增删
来源：http://baike.tarul.cn/Article/details/gdadppmln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/gxquvigof.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/grtehutyv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gyhmpfuuz.sHtML

[S35] C++：map
来源：http://wap.epnwcf.com/Article/details/gnghwsdfn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gtpjbhskx.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/gswpkctmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/ghfccydck.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gtbwzlfol.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/guyamzqtv.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gcnnzxdoc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/ghjjpetqg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/geiqjpywy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gxmjbuabc.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gtlcjeovq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.sjlbkw.cn/Article/details/gisqpjeyv.sHtML


<!-- 参考信息 -->