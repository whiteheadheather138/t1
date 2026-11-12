代发 wailian999

[Q44] IN 子查询
来源：http://wet.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://puo.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://waq.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pwf.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://bxb.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idp.ehwqpu.com

[Q47] 与平均值比较
来源：http://vfs.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opo.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://rgj.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rfc.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://pvz.fengsongda.top

[Q49] 更新单行
来源：http://tdl.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sac.fengsongda.top

[Q50] 批量更新
来源：http://vnk.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sff.cashguo.top

[Q51] 用子查询更新
来源：http://vld.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czg.gaohongyu789.top

[Q52] 删除指定行
来源：http://oor.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://bwr.zdqjudy.top

[Q53] 按条件删除
来源：http://dhv.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rnt.xziqi.cn

[Q54] 清空表
来源：http://kor.hnqzz.top

TRUNCATE TABLE logs;
来源：http://thf.fzhhl.top

[Q55] 排名（并列占位）
来源：http://gmr.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iof.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://ycf.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hni.pycfn.com

[Q57] 行号
来源：http://agb.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lsr.jqgufenzy.top

[Q58] 累计求和
来源：http://vev.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bfi.chenlongwang.top

[Q59] 分组内累计
来源：http://rui.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jnv.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://isp.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jjw.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxl.52xcode.cn

[Q61] 移动平均
来源：http://qcf.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yqk.vehdjk.com

[Q62] 分组占比
来源：http://hsz.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lzk.feifeiyinyue.top

[Q63] 开启事务
来源：http://jxt.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ggw.xinyue.icu

[Q64] 提交事务
来源：http://ikn.yueranfly.top

COMMIT;
来源：http://afz.jinqigufen.top

[Q65] 回滚事务
来源：http://dkr.zdqjudy.top

ROLLBACK;
来源：http://wqo.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://vkn.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uwq.dianchejie.cn

[Q67] 设置隔离级别
来源：http://jna.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mwx.tarul.cn

[Q68] 保存点
来源：http://chy.guannengcc.top

SAVEPOINT sp1;
来源：http://jaf.chenlongwang.top

ROLLBACK TO sp1;
来源：http://ugq.hysaishi.cn

[Q69] 查看执行计划
来源：http://cxv.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vrf.jqgufenzy.top

[Q70] 更新统计信息
来源：http://omr.52xcode.cn

ANALYZE TABLE users;
来源：http://cem.jiagoushi.top

[Q71] 查看建表语句
来源：http://hao.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qgf.bbcook.cn

[Q72] 查看索引
来源：http://jjl.epnwcf.com

SHOW INDEX FROM users;
来源：http://tpp.jianghu66.top

[Q73] 查看表状态
来源：http://qaq.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rbv.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://gwg.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uip.gogol.net.cn

[Q75] 日期格式化
来源：http://irc.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://coc.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://via.jinqigfzy.top

[Q76] 按天统计
来源：http://qkw.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vrh.hammf.cn

[Q77] 时间加减
来源：http://nrl.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lal.cashguo.top

[Q78] 当前时间
来源：http://dzg.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aku.ivvv.top

[Q79] 字符串拼接
来源：http://woj.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gbi.yanxiufei.cn

[Q80] 字符串截取
来源：http://kuy.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lrm.bbcook.cn

[Q81] 字符串替换
来源：http://ifz.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ceq.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://zam.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zmd.yj20258.top

[Q83] 大小写转换
来源：http://sbr.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iya.mhx1999.top

[Q84] 去除首尾空格
来源：http://oae.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://vri.mhx1999.top

[Q85] 数值取整
来源：http://kal.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xum.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://ciz.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tdh.c1oappe.top

[Q87] JSON 字段做条件
来源：http://lcv.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://osu.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://dnt.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hvt.zycfv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://iqi.52xcode.cn

[Q89] 判断表是否存在
来源：http://asl.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fkq.daxiang520.top

[Q90] 生成序号列
来源：http://ndh.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ath.zhongyouzk.top

================================================================================
来源：http://ddc.birdmap.top

R. Bash 专题
来源：http://zlu.tarul.cn

================================================================================
来源：http://wii.vehdjk.com

[R01] shebang 与严格模式
来源：http://yex.snrcjt.cn

#!/usr/bin/env bash
来源：http://ims.fengsongda.top

set -euo pipefail
来源：http://uct.xinyue.icu

[R02] 变量赋值与使用
来源：http://oij.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://kch.bjfxy.top

[R03] 只读变量
来源：http://jbz.yongpay.top

readonly PI=3.14
来源：http://jmv.cdnleiting.top

[R04] 位置参数
来源：http://ixk.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ipb.vqdsnc.cn

[R05] 参数默认值
来源：http://gbs.haohaochexian.top

name="${1:-default}"
来源：http://ocm.sxryk.cn

[R06] 判断命令是否存在
来源：http://pwd.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wxq.redwolf501.top

[R07] if 判断文件
来源：http://cfx.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://abb.ppjwa.cn

[R08] 数值比较
来源：http://goh.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nuu.gaohongyu789.top

[R09] 字符串比较
来源：http://cog.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xbk.kuanghao11.cn

[R10] 正则匹配
来源：http://cof.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tju.xziqi.cn

[R11] case 多分支
来源：http://aeo.bjfxy.top

case "$1" in
来源：http://qbi.ydjk.org.cn

start) echo "启动" ;;
来源：http://gfd.daria6918.cn

stop)  echo "停止" ;;
来源：http://smv.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://spa.zhixingplan.top

esac
来源：http://gbg.hnxiangtu.top

[R12] for 遍历文件
来源：http://bah.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://kme.daria6918.cn

[R13] for 计数循环
来源：http://ocs.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://wla.zdqjudy.top

[R14] C 风格 for
来源：http://twb.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ndn.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://nti.aizwys.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fhq.hysaishi.cn

[R16] until 等待条件
来源：http://ypd.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lch.fzhhl.top

[R17] 数组定义与取值
来源：http://pts.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://prk.fktsv.cn

[R18] 遍历数组
来源：http://isx.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ovp.feifeiyinyue.top

[R19] 数组长度
来源：http://efz.jinqigfzy.top

echo "${#arr[@]}"
来源：http://lvb.yj20258.top

[R20] 关联数组（字典）
来源：http://xsl.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://upi.andypj.xyz

[R21] 字符串长度
来源：http://xdv.gogol.net.cn

echo "${#s}"
来源：http://jll.andypj.xyz

[R22] 截取子串
来源：http://oim.ivvv.top

echo "${s:0:5}"
来源：http://fua.jinqigufen.top

[R23] 字符串替换
来源：http://jbj.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uyj.havefunace.top

[R24] 大小写转换
来源：http://jdo.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uxd.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://gtq.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eqw.chenjidiqi.icu

[R26] 命令替换
来源：http://unh.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://dvq.chenjidiqi.icu

[R27] 算术展开
来源：http://vsa.yonumen.top

echo $((1 + 2 * 3))
来源：http://drz.ydjk.org.cn

[R28] 浮点运算
来源：http://dhl.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://fba.zhoulong.xyz

[R29] 定义函数
来源：http://hhb.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://noa.ctjpmb.com

[R30] 函数返回状态码
来源：http://gyz.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://jyj.shanyushiyangtech.top

[R31] 局部变量
来源：http://mdp.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://zus.havefunace.top

[R32] 参数个数校验
来源：http://bre.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oie.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://nfh.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://etj.ivvv.top

[R34] 退出时清理
来源：http://ovp.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://ivu.aibaodan.cn

[R35] 后台执行并等待
来源：http://qio.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hyk.sysykeji.top

[R36] 并发执行多个任务
来源：http://wbc.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wdu.52xcode.cn

[R37] 把输出赋给变量
来源：http://maz.shanyushiyangkeji.top

files=$(ls -1)
来源：http://ogf.yanxiufei.cn

[R38] 管道串联
来源：http://myy.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://aca.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://she.jqgfzy.top

cmd > out.log 2>&1
来源：http://mcx.cucudq.cn

[R40] 追加写日志
来源：http://zbv.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://uln.sufxvd.cn

[R41] 丢弃输出
来源：http://uxh.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://uxb.cqqwz.cn

[R42] 输入重定向
来源：http://rlg.cdnleiting.top

wc -l < a.txt
来源：http://fmz.bjfxy.top

[R43] 按名字查找文件
来源：http://kwb.cucudq.cn

find . -name "*.log" -type f
来源：http://ctt.zdbjq.cn

[R44] 按修改时间查找
来源：http://wqg.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://yjz.daxiang520.top

[R45] 批量删除
来源：http://een.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://sud.jinqigufen.top

[R46] 递归替换文件内容
来源：http://nox.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ubm.nwbrower.top

[R47] sed 单行替换
来源：http://wih.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ood.jqgfzy.top

[R48] awk 取指定列
来源：http://hki.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://uqi.52xcode.cn

[R49] awk 带条件
来源：http://agw.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://siv.zycfv.cn

[R50] awk 求和
来源：http://mar.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://nod.gogol.net.cn

[R51] 排序去重取前几
来源：http://ltw.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bcw.meibo888.top

[R52] 统计行数
来源：http://ycy.shuidangran.top

wc -l a.txt
来源：http://xki.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://ejr.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pqr.sjlbkw.cn

[R54] 比较两个文件
来源：http://xnz.yangfankeji.com

diff a.txt b.txt
来源：http://upe.cheryme.top

[R55] 压缩与解压
来源：http://fpq.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kfh.andypj.xyz

[R56] 远程拷贝
来源：http://aha.gzhubu.top

scp file user@host:/path/
来源：http://mmq.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://mao.9152youxi.cn

ssh user@host 'uptime'
来源：http://glz.hesvh.cn

[R58] 下载文件
来源：http://wmq.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stl.cashguo.top

[R59] 发 POST JSON
来源：http://bfi.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xqt.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://whd.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ujk.vqdsnc.cn

[R61] 磁盘占用
来源：http://yfl.bjfxy.top

df -h;  du -sh *
来源：http://pbq.cucudq.cn

[R62] 找最占空间的文件
来源：http://kvl.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://egx.zhixingplan.top

[R63] 内存与进程
来源：http://uvf.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://cdw.hesvh.cn

[R64] 结束进程
来源：http://uet.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://obq.quarkkingdee.top

[R65] 查看端口占用
来源：http://yhz.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hce.gaohongyu789.top

[R66] 定时任务
来源：http://kez.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://anp.zycfv.cn

[R67] 生成随机十六进制串
来源：http://evu.zdqjudy.top

openssl rand -hex 16
来源：http://are.dashuyun.cn

[R68] 计算文件校验值
来源：http://ehe.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dhz.316326.xyz

[R69] 生成随机密码
来源：http://kzv.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://hin.daxiang520.top

[R70] 时间戳与互转
来源：http://yyk.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://etp.sufxvd.cn

[R71] 日期格式化
来源：http://udl.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kpf.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://snz.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kgo.kuanghao11.cn

[R73] 分割大日志
来源：http://afo.hywenlv.cn

split -l 1000 big.log part_
来源：http://skr.daxiang520.top

[R74] 批量重命名
来源：http://gak.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kxy.jyoumei.cn

[R75] 导出环境变量
来源：http://fnk.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://ymw.tarul.cn

[R76] 使用临时文件
来源：http://jsm.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fme.sxryk.cn

[R77] 读取用户输入
来源：http://jrl.zhijiandao.cn

read -rp "请输入: " ans
来源：http://yre.yuanzhike.top

[R78] 交互式菜单
来源：http://ghk.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://run.yonumen.top

[R79] 解析命令行选项
来源：http://lrx.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsu.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://qrm.zhaomingkeji.xyz

time ./run.sh
来源：http://fhj.yangfankeji.com

================================================================================
来源：http://jbd.mhx1999.top

S. C / C++ 专题
来源：http://dtv.snrcjt.cn

================================================================================
来源：http://tpj.hnxiangtu.top

[S01] C：Hello World
来源：http://ovx.yueranfly.top

#include <stdio.h>
来源：http://ckf.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://kqk.nwbrower.top

[S02] C：变量与格式化输出
来源：http://qaz.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://hhh.pycfn.com

[S03] C：读入整数
来源：http://vgj.yueranfly.top

int x; scanf("%d", &x);
来源：http://sxf.hfpthk.cn

[S04] C：字符串复制
来源：http://mqq.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://ngm.zdbjq.cn

[S05] C：字符串长度
来源：http://asx.vqdsnc.cn

strlen(s)
来源：http://wmr.sufxvd.cn

[S06] C：字符串比较
来源：http://buc.zdbjq.cn

strcmp(a, b) == 0
来源：http://wwc.tarul.cn

[S07] C：数组遍历求和
来源：http://xtq.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jga.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://bwg.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tgq.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://uhf.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tkl.cheryme.top

[S10] C：指针与解引用
来源：http://igz.daria6918.cn

int *p = &a;  *p = 5;
来源：http://bdy.nanxinkj.top

[S11] C：逐行读文件
来源：http://drk.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://ccv.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vdt.jqgfzy.top

fclose(f);
来源：http://kvl.zhaomingkeji.xyz

[S12] C：写文件
来源：http://rnr.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihe.daria6918.cn

[S13] C：宏定义
来源：http://xna.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kfu.bjfxy.top

[S14] C：枚举
来源：http://abr.dashuyun.cn


<!-- 参考信息 -->