代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://qpe.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://byg.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://vdb.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ktg.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dax.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dhq.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bhw.cqqwz.cn

[Q41] 多表连接
来源：http://tmb.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ewm.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://hpl.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://urk.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://ywn.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://tcq.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nhy.xylfe.cn

[Q43] 标量子查询
来源：http://hmp.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zlw.ctjpmb.com

[Q44] IN 子查询
来源：http://tdx.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hgc.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://yme.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfa.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://jpn.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ecm.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://irr.mhx1999.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://byc.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://pjl.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wat.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://lcs.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://zqi.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://smx.zhongyouzk.top

[Q50] 批量更新
来源：http://hbs.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vum.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://mfd.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lae.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://ogs.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://vvh.zhongyouzk.top

[Q53] 按条件删除
来源：http://biu.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://anz.iojbl.cn

[Q54] 清空表
来源：http://rmi.ydzc1.top

TRUNCATE TABLE logs;
来源：http://eww.tian-w.cn

[Q55] 排名（并列占位）
来源：http://aps.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wvr.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://aqx.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nnt.sweek.top

[Q57] 行号
来源：http://aoa.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://knu.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://tjv.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gah.jinqigfzy.top

[Q59] 分组内累计
来源：http://alk.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gsv.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://ohq.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zwd.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zlp.c1oappe.top

[Q61] 移动平均
来源：http://vay.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sht.svipenyu.cn

[Q62] 分组占比
来源：http://eoa.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bfb.xuetiantiany.cn

[Q63] 开启事务
来源：http://btu.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aww.smart0.xyz

[Q64] 提交事务
来源：http://jos.fanxiaobao.xyz

COMMIT;
来源：http://ior.fzhhl.top

[Q65] 回滚事务
来源：http://kke.daxiang520.top

ROLLBACK;
来源：http://bxb.gogol.net.cn

[Q66] 行锁查询
来源：http://njx.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ycx.tian-w.cn

[Q67] 设置隔离级别
来源：http://ghe.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fxr.chenlongwang.top

[Q68] 保存点
来源：http://oor.cdnleiting.top

SAVEPOINT sp1;
来源：http://skn.hywenlv.cn

ROLLBACK TO sp1;
来源：http://nqb.bbcook.cn

[Q69] 查看执行计划
来源：http://cmn.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mjg.wangdashe.top

[Q70] 更新统计信息
来源：http://sdm.birdmap.top

ANALYZE TABLE users;
来源：http://gvi.yuanzhike.top

[Q71] 查看建表语句
来源：http://ppd.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ncq.nanxuanxn.top

[Q72] 查看索引
来源：http://hxr.hysaishi.cn

SHOW INDEX FROM users;
来源：http://iiy.hnxiangtu.top

[Q73] 查看表状态
来源：http://mpr.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://esr.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://xps.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jaw.shangyingyoupin.top

[Q75] 日期格式化
来源：http://bsf.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bhy.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gid.dashuyun.cn

[Q76] 按天统计
来源：http://tyh.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rnd.havefunace.top

[Q77] 时间加减
来源：http://ubl.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://diq.ybcxt.top

[Q78] 当前时间
来源：http://ekc.yangfankeji.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://prq.yueranfly.top

[Q79] 字符串拼接
来源：http://pbc.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ipn.vehdjk.com

[Q80] 字符串截取
来源：http://ynv.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dbt.ehwqpu.com

[Q81] 字符串替换
来源：http://ddt.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fze.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://xrh.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yyx.yj202588.top

[Q83] 大小写转换
来源：http://rie.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://avc.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://cfu.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://oig.sxryk.cn

[Q85] 数值取整
来源：http://ivm.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uzp.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://rmh.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://enj.bbcook.cn

[Q87] JSON 字段做条件
来源：http://lsf.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kpn.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://szu.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ybs.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hui.zdqjudy.top

[Q89] 判断表是否存在
来源：http://vvo.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qoa.yj20258888.top

[Q90] 生成序号列
来源：http://tlt.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eou.nanxuanxn.top

================================================================================
来源：http://kpc.sjlbkw.cn

R. Bash 专题
来源：http://ldc.sysykeji.top

================================================================================
来源：http://aqv.xuanzx.com

[R01] shebang 与严格模式
来源：http://rso.redwolf501.top

#!/usr/bin/env bash
来源：http://wut.fanxiaobao.xyz

set -euo pipefail
来源：http://yzt.gogol.net.cn

[R02] 变量赋值与使用
来源：http://gws.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://njh.yuxming.cn

[R03] 只读变量
来源：http://myx.svipenyu.cn

readonly PI=3.14
来源：http://ogw.yj20258888.top

[R04] 位置参数
来源：http://zdy.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://akb.pengpengdd.cyou

[R05] 参数默认值
来源：http://kjy.sxryk.cn

name="${1:-default}"
来源：http://hyu.cheryme.top

[R06] 判断命令是否存在
来源：http://ysw.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vrm.gaohongyu789.top

[R07] if 判断文件
来源：http://mtj.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ffj.feifeiyinyue.top

[R08] 数值比较
来源：http://cwv.jianghu66.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qab.haohaochexian.top

[R09] 字符串比较
来源：http://klu.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gak.gzhubu.top

[R10] 正则匹配
来源：http://cqh.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ayy.gaohongyu789.top

[R11] case 多分支
来源：http://ozl.bjfxy.top

case "$1" in
来源：http://fue.snrcjt.cn

start) echo "启动" ;;
来源：http://wce.gogol.net.cn

stop)  echo "停止" ;;
来源：http://zeh.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://uge.jianghu66.top

esac
来源：http://qcp.sweek.top

[R12] for 遍历文件
来源：http://rjr.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://fus.shanyushiyangtech.top

[R13] for 计数循环
来源：http://sxp.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://djs.shanyushiyangtech.top

[R14] C 风格 for
来源：http://gwp.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://grp.0kj1m.cn

[R15] while 逐行读文件
来源：http://xok.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ljj.ybcxt.top

[R16] until 等待条件
来源：http://eej.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://naf.hesvh.cn

[R17] 数组定义与取值
来源：http://aeo.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sik.chenjidiqi.icu

[R18] 遍历数组
来源：http://afx.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dmp.dashuyun.cn

[R19] 数组长度
来源：http://ogc.sysykeji.top

echo "${#arr[@]}"
来源：http://vbb.shuidangran.top

[R20] 关联数组（字典）
来源：http://boi.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xyd.kuanghao11.cn

[R21] 字符串长度
来源：http://uqq.zhijiandao.cn

echo "${#s}"
来源：http://fbv.tianlin.xyz

[R22] 截取子串
来源：http://ebr.redwolf501.top

echo "${s:0:5}"
来源：http://qmn.redwolf501.top

[R23] 字符串替换
来源：http://lht.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hpc.jlsjyb.cn

[R24] 大小写转换
来源：http://wty.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://dot.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://emo.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://dvy.tarul.cn

[R26] 命令替换
来源：http://dku.yj202588.top

now=$(date +%F); echo "$now"
来源：http://izq.tianlin.xyz

[R27] 算术展开
来源：http://jhv.cheryme.top

echo $((1 + 2 * 3))
来源：http://gaj.aibaodan.cn

[R28] 浮点运算
来源：http://fbp.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://wmy.dashuyun.cn

[R29] 定义函数
来源：http://hbm.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hjb.yj202588.top

[R30] 函数返回状态码
来源：http://aqh.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://yyb.bbcook.cn

[R31] 局部变量
来源：http://qgy.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://ndo.xinyue.icu

[R32] 参数个数校验
来源：http://knd.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xat.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://kwp.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tfa.hnqzz.top

[R34] 退出时清理
来源：http://mbq.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://ikz.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://nqq.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hyv.shzxlz.cn

[R36] 并发执行多个任务
来源：http://dew.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fiz.ivvv.top

[R37] 把输出赋给变量
来源：http://lfn.hnqzz.top

files=$(ls -1)
来源：http://iyb.jianghu66.top

[R38] 管道串联
来源：http://akx.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://lxl.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://yhr.fktsv.cn

cmd > out.log 2>&1
来源：http://xjt.hammf.cn

[R40] 追加写日志
来源：http://zqb.sweek.top

echo "log" >> out.log
来源：http://ttd.xuetiantiany.cn

[R41] 丢弃输出
来源：http://rrk.meibo888.top

cmd >/dev/null 2>&1
来源：http://bnr.shangyingyoupin.top

[R42] 输入重定向
来源：http://ayj.havefunace.top

wc -l < a.txt
来源：http://ila.yonumen.top

[R43] 按名字查找文件
来源：http://uhh.uphjek.com

find . -name "*.log" -type f
来源：http://amq.yvedp.cn

[R44] 按修改时间查找
来源：http://wbn.wangdashe.top

find . -mtime -7 -type f
来源：http://mem.ehwqpu.com

[R45] 批量删除
来源：http://xzf.wangdashe.top

find . -name "*.tmp" -delete
来源：http://llo.ivvv.top

[R46] 递归替换文件内容
来源：http://han.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qdd.aizwys.cn

[R47] sed 单行替换
来源：http://ryc.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://mda.tanke756.top

[R48] awk 取指定列
来源：http://dfl.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://aos.ehwqpu.com

[R49] awk 带条件
来源：http://pno.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lte.chenjidiqi.icu

[R50] awk 求和
来源：http://keo.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://uem.quarkkingdee.top

[R51] 排序去重取前几
来源：http://dzo.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://opy.mhx1999.top

[R52] 统计行数
来源：http://adp.vehdjk.com

wc -l a.txt
来源：http://ejm.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://gjp.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pty.wangshuangyany.cn

[R54] 比较两个文件
来源：http://mvc.gotoacloud.top

diff a.txt b.txt
来源：http://scr.zhengqikj.top

[R55] 压缩与解压
来源：http://knt.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mcg.jiagoushi.top

[R56] 远程拷贝
来源：http://ooi.jianghu66.top

scp file user@host:/path/
来源：http://vkx.xinyue.icu

[R57] 远程执行命令
来源：http://kqg.hysaishi.cn

ssh user@host 'uptime'
来源：http://yho.c1oappe.top

[R58] 下载文件
来源：http://wac.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jdl.vehdjk.com

[R59] 发 POST JSON
来源：http://lwd.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jug.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://tvu.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ett.tianlin.xyz

[R61] 磁盘占用
来源：http://kjs.epnwcf.com

df -h;  du -sh *
来源：http://baf.redwolf501.top

[R62] 找最占空间的文件
来源：http://tfx.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://ehn.bjfxy.top

[R63] 内存与进程
来源：http://qva.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://xhi.hnqzz.top

[R64] 结束进程
来源：http://mhv.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://gbe.smart0.xyz

[R65] 查看端口占用
来源：http://zdj.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tuh.fktsv.cn

[R66] 定时任务
来源：http://cso.316326.xyz

crontab -e;  crontab -l
来源：http://quu.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://plc.andypj.xyz

openssl rand -hex 16
来源：http://uck.mhx1999.top

[R68] 计算文件校验值
来源：http://wev.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tth.aizwys.cn

[R69] 生成随机密码
来源：http://ovf.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://xlc.tarul.cn

[R70] 时间戳与互转
来源：http://zgj.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://ntq.vqdsnc.cn

[R71] 日期格式化
来源：http://mxz.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ufy.snrcjt.cn

[R72] 等待端口就绪
来源：http://ncq.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yma.cheryme.top

[R73] 分割大日志
来源：http://syl.xziqi.cn

split -l 1000 big.log part_
来源：http://mpc.hnqzz.top

[R74] 批量重命名
来源：http://jaz.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fra.sysykeji.top

[R75] 导出环境变量
来源：http://eun.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://tnw.cashguo.top

[R76] 使用临时文件
来源：http://mbi.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wve.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://sux.yfazqb.com

read -rp "请输入: " ans
来源：http://tar.zhiwuduotai.top

[R78] 交互式菜单
来源：http://ite.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://idn.chenlongwang.top

[R79] 解析命令行选项
来源：http://rii.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rfm.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://gnf.zycfv.cn

time ./run.sh
来源：http://ugf.bbcook.cn

================================================================================
来源：http://aah.tian-w.cn

S. C / C++ 专题
来源：http://vuo.shangyingyoupin.top

================================================================================
来源：http://iaj.svipenyu.cn

[S01] C：Hello World
来源：http://ltx.hnxiangtu.top

#include <stdio.h>
来源：http://wwj.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fcs.52xcode.cn

[S02] C：变量与格式化输出
来源：http://kfv.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://ukh.dianchejie.cn

[S03] C：读入整数
来源：http://avk.zhixingplan.top

int x; scanf("%d", &x);
来源：http://btf.jinqigfzy.top

[S04] C：字符串复制
来源：http://bda.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://hmj.cucudq.cn

[S05] C：字符串长度
来源：http://snm.svipenyu.cn

strlen(s)
来源：http://eny.wangshuangyany.cn

[S06] C：字符串比较
来源：http://ecp.dashuyun.cn

strcmp(a, b) == 0
来源：http://pnb.yangfankeji.com

[S07] C：数组遍历求和
来源：http://hxg.yangfankeji.com


<!-- 参考信息 -->