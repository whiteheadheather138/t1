代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://qup.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://hhe.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://gws.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://vxn.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://tsf.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ebw.sufxvd.cn

[Q43] 标量子查询
来源：http://bpb.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zde.chenzaomai.com

[Q44] IN 子查询
来源：http://svk.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wen.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://wfq.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nnd.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://jyv.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agp.ivvv.top

[Q47] 与平均值比较
来源：http://uid.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dwc.yj20258.top

[Q48] CTE 公用表表达式
来源：http://csb.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fkl.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://tbl.xinyue.icu

[Q49] 更新单行
来源：http://qsb.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kmr.ctjpmb.com

[Q50] 批量更新
来源：http://jna.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kxd.xuanzx.com

[Q51] 用子查询更新
来源：http://fhj.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ivx.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://tsz.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://dxg.hfpthk.cn

[Q53] 按条件删除
来源：http://ggo.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ikf.fengsongda.top

[Q54] 清空表
来源：http://wgr.316326.xyz

TRUNCATE TABLE logs;
来源：http://qfw.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://fti.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jmy.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://dnp.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ray.cqqwz.cn

[Q57] 行号
来源：http://qsn.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vlk.ydzc1.top

[Q58] 累计求和
来源：http://cxw.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mzy.yonumen.top

[Q59] 分组内累计
来源：http://sxk.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ebj.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://xix.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://axo.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jru.yueranfly.top

[Q61] 移动平均
来源：http://zhw.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gds.hammf.cn

[Q62] 分组占比
来源：http://ucy.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mww.dianchejie.cn

[Q63] 开启事务
来源：http://wip.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kjw.smart0.xyz

[Q64] 提交事务
来源：http://ipz.jianghu66.top

COMMIT;
来源：http://qla.fzhhl.top

[Q65] 回滚事务
来源：http://qrt.guannengcc.top

ROLLBACK;
来源：http://cdp.shuidangran.top

[Q66] 行锁查询
来源：http://lgz.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ayo.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://enw.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ozb.9152youxi.cn

[Q68] 保存点
来源：http://koq.uphjek.com

SAVEPOINT sp1;
来源：http://lgc.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://iip.haohaochexian.top

[Q69] 查看执行计划
来源：http://cuo.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zwh.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://hhc.ctjpmb.com

ANALYZE TABLE users;
来源：http://bqp.vehdjk.com

[Q71] 查看建表语句
来源：http://ehc.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwy.andypj.xyz

[Q72] 查看索引
来源：http://xwm.sxryk.cn

SHOW INDEX FROM users;
来源：http://kqq.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://mcx.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pjf.guannengcc.top

[Q74] 强制使用索引
来源：http://byr.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oxj.zhongyouzk.top

[Q75] 日期格式化
来源：http://lqb.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fmk.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fix.hywenlv.cn

[Q76] 按天统计
来源：http://sij.zycfv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hft.meibo888.top

[Q77] 时间加减
来源：http://djp.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rqy.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://hwz.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zgm.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://rrc.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qep.quarkkingdee.top

[Q80] 字符串截取
来源：http://mln.ehwqpu.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eri.jinqigufen.top

[Q81] 字符串替换
来源：http://qvx.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ckv.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://xpv.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dqt.cdnleiting.top

[Q83] 大小写转换
来源：http://bdg.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bnh.ctjpmb.com

[Q84] 去除首尾空格
来源：http://mtt.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://qjh.ydzc1.top

[Q85] 数值取整
来源：http://wwq.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ydx.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://gmd.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vpc.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://opq.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://opf.pycfn.com

[Q88] 行转列（条件聚合）
来源：http://fnr.wangshuangyany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://own.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sus.yuanzhike.top

[Q89] 判断表是否存在
来源：http://ufh.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xxe.hongshengwenyu.top

[Q90] 生成序号列
来源：http://jie.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rkc.pycfn.com

================================================================================
来源：http://cnf.cqqwz.cn

R. Bash 专题
来源：http://prc.jinyuanbaomall.cn

================================================================================
来源：http://yby.redwolf501.top

[R01] shebang 与严格模式
来源：http://njm.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://yii.zhixingplan.top

set -euo pipefail
来源：http://zrs.cdnleiting.top

[R02] 变量赋值与使用
来源：http://dot.tanke756.top

name="Tom"; echo "$name"
来源：http://rsz.redwolf501.top

[R03] 只读变量
来源：http://oab.jianghu66.top

readonly PI=3.14
来源：http://wrc.shuidangran.top

[R04] 位置参数
来源：http://muk.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zca.hesvh.cn

[R05] 参数默认值
来源：http://uiq.mhx1999.top

name="${1:-default}"
来源：http://hqz.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://hxi.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lnp.feifeiyinyue.top

[R07] if 判断文件
来源：http://hrl.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pzq.gzhubu.top

[R08] 数值比较
来源：http://mrz.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lok.kuanghao11.cn

[R09] 字符串比较
来源：http://uxx.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://frg.iojbl.cn

[R10] 正则匹配
来源：http://xbj.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uxu.uphjek.com

[R11] case 多分支
来源：http://pyb.zdqjudy.top

case "$1" in
来源：http://keg.ybcxt.top

start) echo "启动" ;;
来源：http://xwg.316326.xyz

stop)  echo "停止" ;;
来源：http://ybl.yfazqb.com

*)     echo "未知命令" ;;
来源：http://imj.svipenyu.cn

esac
来源：http://ynl.hnxiangtu.top

[R12] for 遍历文件
来源：http://zjx.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://ozt.yuxming.cn

[R13] for 计数循环
来源：http://jel.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://gck.zhongyouzk.top

[R14] C 风格 for
来源：http://zgw.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://viq.sjlbkw.cn

[R15] while 逐行读文件
来源：http://qxv.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wfy.cashguo.top

[R16] until 等待条件
来源：http://xfc.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nwj.ehwqpu.com

[R17] 数组定义与取值
来源：http://pii.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://adg.xuetiantiany.cn

[R18] 遍历数组
来源：http://vhs.aibaodan.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rkt.zhoulong.xyz

[R19] 数组长度
来源：http://qkp.fehbvm.com

echo "${#arr[@]}"
来源：http://vbb.fzhhl.top

[R20] 关联数组（字典）
来源：http://upn.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tkv.smart0.xyz

[R21] 字符串长度
来源：http://nqg.yueranfly.top

echo "${#s}"
来源：http://top.jqgufenzy.top

[R22] 截取子串
来源：http://pxf.bjfxy.top

echo "${s:0:5}"
来源：http://kkw.svipenyu.cn

[R23] 字符串替换
来源：http://azx.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tlp.pengpengdd.cyou

[R24] 大小写转换
来源：http://ysp.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://vnm.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://zbz.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dyi.iojbl.cn

[R26] 命令替换
来源：http://pkt.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://alo.shangyingyoupin.top

[R27] 算术展开
来源：http://yey.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://svt.jyoumei.cn

[R28] 浮点运算
来源：http://gyg.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://kke.mhx1999.top

[R29] 定义函数
来源：http://vgv.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mso.ybcxt.top

[R30] 函数返回状态码
来源：http://yjg.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://nno.svipenyu.cn

[R31] 局部变量
来源：http://qdo.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://lmn.ctjpmb.com

[R32] 参数个数校验
来源：http://cak.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nqo.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://piw.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yhp.gzhubu.top

[R34] 退出时清理
来源：http://oew.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://gnu.sufxvd.cn

[R35] 后台执行并等待
来源：http://led.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://jjy.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://kng.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uhw.tarul.cn

[R37] 把输出赋给变量
来源：http://yau.yfazqb.com

files=$(ls -1)
来源：http://hii.vehdjk.com

[R38] 管道串联
来源：http://tpv.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://sda.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://icc.vehdjk.com

cmd > out.log 2>&1
来源：http://apj.sjlbkw.cn

[R40] 追加写日志
来源：http://smh.316326.xyz

echo "log" >> out.log
来源：http://zab.zhiwuduotai.top

[R41] 丢弃输出
来源：http://orp.gzhubu.top

cmd >/dev/null 2>&1
来源：http://cfk.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://rms.xinyue.icu

wc -l < a.txt
来源：http://vbl.sufxvd.cn

[R43] 按名字查找文件
来源：http://one.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://mku.hywenlv.cn

[R44] 按修改时间查找
来源：http://xau.cashguo.top

find . -mtime -7 -type f
来源：http://ejq.yfazqb.com

[R45] 批量删除
来源：http://nas.cheryme.top

find . -name "*.tmp" -delete
来源：http://cyq.bjfxy.top

[R46] 递归替换文件内容
来源：http://wzr.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zst.xziqi.cn

[R47] sed 单行替换
来源：http://hre.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://sis.fzhhl.top

[R48] awk 取指定列
来源：http://ffp.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://jnn.yonumen.top

[R49] awk 带条件
来源：http://iit.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cjf.aizwys.cn

[R50] awk 求和
来源：http://joa.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://jia.sweek.top

[R51] 排序去重取前几
来源：http://nbf.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nmk.jiagoushi.top

[R52] 统计行数
来源：http://gre.jinqigfzy.top

wc -l a.txt
来源：http://efm.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://hbk.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vde.svipenyu.cn

[R54] 比较两个文件
来源：http://dcq.zhoulong.xyz

diff a.txt b.txt
来源：http://btv.smart0.xyz

[R55] 压缩与解压
来源：http://wnw.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vnf.jlsjyb.cn

[R56] 远程拷贝
来源：http://hav.nwbrower.top

scp file user@host:/path/
来源：http://pnh.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://hjn.yj20258888.top

ssh user@host 'uptime'
来源：http://lut.hnqzz.top

[R58] 下载文件
来源：http://skp.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yev.dianchejie.cn

[R59] 发 POST JSON
来源：http://api.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tzh.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://oqp.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xjz.gzhubu.top

[R61] 磁盘占用
来源：http://zdp.jianghu66.top

df -h;  du -sh *
来源：http://msz.hcnkem.com

[R62] 找最占空间的文件
来源：http://rjy.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://etb.yuxming.cn

[R63] 内存与进程
来源：http://ohx.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://bnu.shangyingyoupin.top

[R64] 结束进程
来源：http://rzo.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://hwa.ppjwa.cn

[R65] 查看端口占用
来源：http://xtn.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uxs.zhijiandao.cn

[R66] 定时任务
来源：http://fbw.dashuyun.cn

crontab -e;  crontab -l
来源：http://ltv.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://kiu.yanxiufei.cn

openssl rand -hex 16
来源：http://ntj.tarul.cn

[R68] 计算文件校验值
来源：http://vdn.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://joa.bbcook.cn

[R69] 生成随机密码
来源：http://bue.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://ldn.zhengqikj.top

[R70] 时间戳与互转
来源：http://hxi.fzhhl.top

date +%s;  date -d @1700000000
来源：http://nim.0kj1m.cn

[R71] 日期格式化
来源：http://rfx.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hdq.sxryk.cn

[R72] 等待端口就绪
来源：http://pqh.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fjs.sweek.top

[R73] 分割大日志
来源：http://uzx.haohaochexian.top

split -l 1000 big.log part_
来源：http://lyp.yj20258888.top

[R74] 批量重命名
来源：http://cwb.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vim.yj20258.top

[R75] 导出环境变量
来源：http://hfg.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://yry.9152youxi.cn

[R76] 使用临时文件
来源：http://zox.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://geh.yanxiufei.cn

[R77] 读取用户输入
来源：http://rsn.hammf.cn

read -rp "请输入: " ans
来源：http://hqr.yanxiufei.cn

[R78] 交互式菜单
来源：http://cpr.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zon.gogol.net.cn

[R79] 解析命令行选项
来源：http://uer.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://moa.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://smm.redwolf501.top

time ./run.sh
来源：http://miq.havefunace.top

================================================================================
来源：http://ggh.chenzaomai.com

S. C / C++ 专题
来源：http://kei.yvedp.cn

================================================================================
来源：http://lat.hysaishi.cn

[S01] C：Hello World
来源：http://wec.yonumen.top

#include <stdio.h>
来源：http://cdu.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qpc.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://jca.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://xdv.yanxiufei.cn

[S03] C：读入整数
来源：http://tgz.yj202588.top

int x; scanf("%d", &x);
来源：http://sut.iojbl.cn

[S04] C：字符串复制
来源：http://lcf.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xwd.guannengcc.top

[S05] C：字符串长度
来源：http://jjq.sjlbkw.cn

strlen(s)
来源：http://eto.aizwys.cn

[S06] C：字符串比较
来源：http://ozh.jiagoushi.top

strcmp(a, b) == 0
来源：http://zrx.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://cjn.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uxj.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://poa.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ytt.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://yhy.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kpy.smart0.xyz

[S10] C：指针与解引用
来源：http://qxa.smart0.xyz

int *p = &a;  *p = 5;
来源：http://xwv.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://zwa.epnwcf.com


<!-- 参考信息 -->