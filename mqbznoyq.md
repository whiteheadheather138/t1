代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fgu.zhixingplan.top

[Q28] 求和与平均
来源：http://bsv.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzl.hammf.cn

[Q29] 最大最小值
来源：http://zzg.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dyn.yanxiufei.cn

[Q30] 分组统计
来源：http://gda.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iet.nwbrower.top

[Q31] 分组后过滤
来源：http://yqc.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sug.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://usx.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xxd.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dus.jianghu66.top

[Q33] 多列分组
来源：http://vop.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xqj.gzhubu.top

[Q34] 每组取第一条
来源：http://mkx.c1oappe.top

SELECT * FROM (
来源：http://jmc.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nnj.iojbl.cn

) t WHERE rn = 1;
来源：http://qef.hysaishi.cn

[Q35] 内连接
来源：http://qix.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cew.fktsv.cn

[Q36] 左连接
来源：http://wdn.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qrw.birdmap.top

[Q37] 右连接
来源：http://yvj.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ast.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://pkb.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tmw.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://yae.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://avq.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ebd.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dkv.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wtx.xinyue.icu

[Q41] 多表连接
来源：http://wey.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rbx.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://hww.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://uyy.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://yuo.9152youxi.cn

SELECT u.name, o.amount FROM users u
来源：http://apr.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dsp.dianchejie.cn

[Q43] 标量子查询
来源：http://vyu.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zlk.fktsv.cn

[Q44] IN 子查询
来源：http://eni.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yys.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://ezz.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xvw.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kzg.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qho.cucudq.cn

[Q47] 与平均值比较
来源：http://uih.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://inc.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://chr.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jyl.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://peq.epnwcf.com

[Q49] 更新单行
来源：http://srg.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://svv.sufxvd.cn

[Q50] 批量更新
来源：http://aqz.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://atr.yueranfly.top

[Q51] 用子查询更新
来源：http://hkv.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fwg.gotoacloud.top

[Q52] 删除指定行
来源：http://zxy.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://ows.svipenyu.cn

[Q53] 按条件删除
来源：http://snn.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://djm.xziqi.cn

[Q54] 清空表
来源：http://ymm.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://ynf.hnqzz.top

[Q55] 排名（并列占位）
来源：http://igc.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xmw.iojbl.cn

[Q56] 密集排名（并列不占位）
来源：http://tzc.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oak.cqqwz.cn

[Q57] 行号
来源：http://ybw.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dat.yuxming.cn

[Q58] 累计求和
来源：http://awt.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://joi.svipenyu.cn

[Q59] 分组内累计
来源：http://uhn.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iik.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://nje.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ofy.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://khi.cdnleiting.top

[Q61] 移动平均
来源：http://auj.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://stv.9152youxi.cn

[Q62] 分组占比
来源：http://jgg.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vor.nanxinkj.top

[Q63] 开启事务
来源：http://xko.ydjk.org.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ojz.svipenyu.cn

[Q64] 提交事务
来源：http://cjn.shangyingyoupin.top

COMMIT;
来源：http://kyl.yj202588.top

[Q65] 回滚事务
来源：http://bka.aizwys.cn

ROLLBACK;
来源：http://kzy.shuidangran.top

[Q66] 行锁查询
来源：http://pho.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://btf.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://sgc.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsr.yuanzhike.top

[Q68] 保存点
来源：http://bkp.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://ohr.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://jzg.jyoumei.cn

[Q69] 查看执行计划
来源：http://dyy.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dbg.andypj.xyz

[Q70] 更新统计信息
来源：http://jeb.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://xbj.tian-w.cn

[Q71] 查看建表语句
来源：http://dme.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://msg.ctjpmb.com

[Q72] 查看索引
来源：http://tjj.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://cpm.fengsongda.top

[Q73] 查看表状态
来源：http://zdh.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ebm.quarkkingdee.top

[Q74] 强制使用索引
来源：http://tha.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://clu.gzhubu.top

[Q75] 日期格式化
来源：http://hqh.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yus.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ktg.cashguo.top

[Q76] 按天统计
来源：http://fex.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eyn.bjfxy.top

[Q77] 时间加减
来源：http://dwi.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rlt.pengpengdd.cyou

[Q78] 当前时间
来源：http://iua.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kfv.gzhubu.top

[Q79] 字符串拼接
来源：http://vln.52xcode.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cae.quarkkingdee.top

[Q80] 字符串截取
来源：http://vxe.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hdf.zhiwuduotai.top

[Q81] 字符串替换
来源：http://sox.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lln.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://kan.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blv.vehdjk.com

[Q83] 大小写转换
来源：http://epk.snrcjt.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cwb.ybcxt.top

[Q84] 去除首尾空格
来源：http://ooy.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://wvb.fzhhl.top

[Q85] 数值取整
来源：http://dor.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kfv.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://usy.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://twu.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://lfz.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qwc.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://vul.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jxw.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mzq.ehwqpu.com

[Q89] 判断表是否存在
来源：http://tcl.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wrh.snrcjt.cn

[Q90] 生成序号列
来源：http://kmx.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xye.ydzc1.top

================================================================================
来源：http://ymk.xuanzx.com

R. Bash 专题
来源：http://smb.iojbl.cn

================================================================================
来源：http://jsr.zdbjq.cn

[R01] shebang 与严格模式
来源：http://irx.zhoulong.xyz

#!/usr/bin/env bash
来源：http://yme.xingfuxueyuan.xyz

set -euo pipefail
来源：http://rvn.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://dre.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://klv.hywenlv.cn

[R03] 只读变量
来源：http://lsm.cheryme.top

readonly PI=3.14
来源：http://sdw.yuanzhike.top

[R04] 位置参数
来源：http://vgx.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxf.ehwqpu.com

[R05] 参数默认值
来源：http://qyk.c1oappe.top

name="${1:-default}"
来源：http://smh.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://vep.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rnq.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://kfe.gotoacloud.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lty.xuanzx.com

[R08] 数值比较
来源：http://ync.ivvv.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bzu.jyoumei.cn

[R09] 字符串比较
来源：http://mvy.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mvf.smart0.xyz

[R10] 正则匹配
来源：http://uih.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qdf.daria6918.cn

[R11] case 多分支
来源：http://xkm.gaohongyu789.top

case "$1" in
来源：http://bxn.xuanzx.com

start) echo "启动" ;;
来源：http://lqx.fzhhl.top

stop)  echo "停止" ;;
来源：http://cjy.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://jbq.zycfv.cn

esac
来源：http://miy.gogol.net.cn

[R12] for 遍历文件
来源：http://fpj.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://xxv.jlsjyb.cn

[R13] for 计数循环
来源：http://xzy.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://zlr.haohaochexian.top

[R14] C 风格 for
来源：http://tso.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zhw.zhijiandao.cn

[R15] while 逐行读文件
来源：http://svn.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uju.ivvv.top

[R16] until 等待条件
来源：http://wzn.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eph.fktsv.cn

[R17] 数组定义与取值
来源：http://tgs.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://gco.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://kab.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujo.jianghu66.top

[R19] 数组长度
来源：http://eic.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://akc.tian-w.cn

[R20] 关联数组（字典）
来源：http://qxh.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fkz.nanxinkj.top

[R21] 字符串长度
来源：http://umr.aibaodan.cn

echo "${#s}"
来源：http://ecy.hongshengwenyu.top

[R22] 截取子串
来源：http://gfy.nwbrower.top

echo "${s:0:5}"
来源：http://wdx.yj20258888.top

[R23] 字符串替换
来源：http://sud.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xyq.shanyushiyangtech.top

[R24] 大小写转换
来源：http://aaf.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://wpe.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://ard.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vwo.cucudq.cn

[R26] 命令替换
来源：http://bye.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://oat.jqgfzy.top

[R27] 算术展开
来源：http://ibc.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://wli.sweek.top

[R28] 浮点运算
来源：http://ysu.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://zdv.chenlongwang.top

[R29] 定义函数
来源：http://pxa.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rxy.cashguo.top

[R30] 函数返回状态码
来源：http://hkw.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://obt.xuanzx.com

[R31] 局部变量
来源：http://tpa.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://oyt.andypj.xyz

[R32] 参数个数校验
来源：http://rvy.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vzy.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://fwe.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://txk.tian-w.cn

[R34] 退出时清理
来源：http://ysn.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://upk.hammf.cn

[R35] 后台执行并等待
来源：http://twk.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qdc.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://gzw.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://epg.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://utv.tarul.cn

files=$(ls -1)
来源：http://cyt.yanxiufei.cn

[R38] 管道串联
来源：http://xnm.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://hmw.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://jsl.0kj1m.cn

cmd > out.log 2>&1
来源：http://ozg.bjfxy.top

[R40] 追加写日志
来源：http://lwg.wangshuangyany.cn

echo "log" >> out.log
来源：http://pvd.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://nov.gzhubu.top

cmd >/dev/null 2>&1
来源：http://ysj.yvedp.cn

[R42] 输入重定向
来源：http://eui.pycfn.com

wc -l < a.txt
来源：http://swx.iojbl.cn

[R43] 按名字查找文件
来源：http://nqq.fengsongda.top

find . -name "*.log" -type f
来源：http://tds.fehbvm.com

[R44] 按修改时间查找
来源：http://qlo.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://gba.xylfe.cn

[R45] 批量删除
来源：http://fjg.fzhhl.top

find . -name "*.tmp" -delete
来源：http://lhi.sysykeji.top

[R46] 递归替换文件内容
来源：http://bai.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxd.aizwys.cn

[R47] sed 单行替换
来源：http://syo.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://nyh.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://udf.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://duz.ydzc1.top

[R49] awk 带条件
来源：http://tio.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oce.yfazqb.com

[R50] awk 求和
来源：http://evf.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://evn.nanxinkj.top

[R51] 排序去重取前几
来源：http://wwe.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nlp.wangshuangyany.cn

[R52] 统计行数
来源：http://kip.ydzc1.top

wc -l a.txt
来源：http://ioc.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://xpz.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vna.xylfe.cn

[R54] 比较两个文件
来源：http://dvi.mhx1999.top

diff a.txt b.txt
来源：http://tvw.bjfxy.top

[R55] 压缩与解压
来源：http://wcy.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qqk.jianghu66.top

[R56] 远程拷贝
来源：http://sri.316326.xyz

scp file user@host:/path/
来源：http://ols.xuanzx.com

[R57] 远程执行命令
来源：http://mpl.jlsjyb.cn

ssh user@host 'uptime'
来源：http://yws.smart0.xyz

[R58] 下载文件
来源：http://pnb.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mqq.iojbl.cn

[R59] 发 POST JSON
来源：http://esq.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://auy.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://ykt.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ezz.hammf.cn

[R61] 磁盘占用
来源：http://lym.ehwqpu.com

df -h;  du -sh *
来源：http://yse.xuanzx.com

[R62] 找最占空间的文件
来源：http://cjn.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://wxz.aizwys.cn

[R63] 内存与进程
来源：http://bfs.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://jmt.jinyuanbaomall.cn

[R64] 结束进程
来源：http://ibq.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://tyg.cucudq.cn

[R65] 查看端口占用
来源：http://qvp.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytm.iojbl.cn

[R66] 定时任务
来源：http://pll.meibo888.top

crontab -e;  crontab -l
来源：http://xap.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://bgj.redwolf501.top

openssl rand -hex 16
来源：http://tlu.sufxvd.cn

[R68] 计算文件校验值
来源：http://cpn.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dfw.daria6918.cn

[R69] 生成随机密码
来源：http://lvp.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://but.shzxlz.cn

[R70] 时间戳与互转
来源：http://lbf.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://bwv.pycfn.com

[R71] 日期格式化
来源：http://wli.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://voe.hesvh.cn

[R72] 等待端口就绪
来源：http://ilr.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ice.tarul.cn

[R73] 分割大日志
来源：http://rga.hywenlv.cn

split -l 1000 big.log part_
来源：http://ths.aibaodan.cn

[R74] 批量重命名
来源：http://epk.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://abe.snrcjt.cn

[R75] 导出环境变量
来源：http://cbq.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://pnr.yonumen.top

[R76] 使用临时文件
来源：http://zyp.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://usy.chenjidiqi.icu

[R77] 读取用户输入
来源：http://gfu.yvedp.cn


<!-- 参考信息 -->