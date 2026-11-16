代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://npr.zdbjq.cn

[Q30] 分组统计
来源：http://ais.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kgy.hcnkem.com

[Q31] 分组后过滤
来源：http://end.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kns.wangshuangyany.cn

[Q32] 分组拼接字符串
来源：http://azf.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ega.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kab.snrcjt.cn

[Q33] 多列分组
来源：http://bpb.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zmr.sweek.top

[Q34] 每组取第一条
来源：http://ksu.hesvh.cn

SELECT * FROM (
来源：http://xjl.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://awu.havefunace.top

) t WHERE rn = 1;
来源：http://dci.zhiwuduotai.top

[Q35] 内连接
来源：http://was.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cgb.mhx1999.top

[Q36] 左连接
来源：http://lka.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hob.dashuyun.cn

[Q37] 右连接
来源：http://frt.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bvj.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://wzu.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jjb.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://ttc.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrt.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vtv.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://sxl.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xao.vqdsnc.cn

[Q41] 多表连接
来源：http://mcf.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cfd.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://uem.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mhy.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://twm.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://vag.hfpthk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sim.zdqjudy.top

[Q43] 标量子查询
来源：http://wva.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uhr.cucudq.cn

[Q44] IN 子查询
来源：http://zoj.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cwl.cheryme.top

[Q45] EXISTS 判断存在
来源：http://fvj.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qva.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xhr.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xto.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://xyc.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eam.tanke756.top

[Q48] CTE 公用表表达式
来源：http://sxw.xinyue.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aus.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://iwa.smart0.xyz

[Q49] 更新单行
来源：http://dgj.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zek.aibaodan.cn

[Q50] 批量更新
来源：http://svo.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uva.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://vui.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yko.fehbvm.com

[Q52] 删除指定行
来源：http://zkf.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://jjx.dashuyun.cn

[Q53] 按条件删除
来源：http://lmu.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pcs.9152youxi.cn

[Q54] 清空表
来源：http://paj.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://ljj.zycfv.cn

[Q55] 排名（并列占位）
来源：http://cas.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvb.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://dgf.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fbj.wangshuangyany.cn

[Q57] 行号
来源：http://kca.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vqu.yueranfly.top

[Q58] 累计求和
来源：http://zvd.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gvq.jlsjyb.cn

[Q59] 分组内累计
来源：http://fyc.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://esb.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://rsi.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pxr.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hqn.chenlongwang.top

[Q61] 移动平均
来源：http://bgb.cdnleiting.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://czy.hfpthk.cn

[Q62] 分组占比
来源：http://awj.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sca.yj202588.top

[Q63] 开启事务
来源：http://aat.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xgd.redwolf501.top

[Q64] 提交事务
来源：http://cng.tanke756.top

COMMIT;
来源：http://yec.meibo888.top

[Q65] 回滚事务
来源：http://oye.hnqzz.top

ROLLBACK;
来源：http://acd.cashguo.top

[Q66] 行锁查询
来源：http://adu.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vkm.yj202588.top

[Q67] 设置隔离级别
来源：http://bhv.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ypt.vehdjk.com

[Q68] 保存点
来源：http://zln.gogol.net.cn

SAVEPOINT sp1;
来源：http://xnd.yvedp.cn

ROLLBACK TO sp1;
来源：http://zib.jyoumei.cn

[Q69] 查看执行计划
来源：http://ywg.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hyx.gogol.net.cn

[Q70] 更新统计信息
来源：http://fft.kuanghao11.cn

ANALYZE TABLE users;
来源：http://sdd.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://dhy.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ipm.uphjek.com

[Q72] 查看索引
来源：http://elg.havefunace.top

SHOW INDEX FROM users;
来源：http://cef.redwolf501.top

[Q73] 查看表状态
来源：http://xdv.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://khp.ivvv.top

[Q74] 强制使用索引
来源：http://adm.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://geo.smart0.xyz

[Q75] 日期格式化
来源：http://kvf.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ynn.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zak.yj20258.top

[Q76] 按天统计
来源：http://aso.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfg.epnwcf.com

[Q77] 时间加减
来源：http://vgx.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hsh.kuanghao11.cn

[Q78] 当前时间
来源：http://bjv.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ijn.bjfxy.top

[Q79] 字符串拼接
来源：http://bcw.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oly.0kj1m.cn

[Q80] 字符串截取
来源：http://sce.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wms.sweek.top

[Q81] 字符串替换
来源：http://may.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pzx.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://aus.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ldu.ydzc1.top

[Q83] 大小写转换
来源：http://dvg.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dtr.ivvv.top

[Q84] 去除首尾空格
来源：http://swd.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://lxt.hysaishi.cn

[Q85] 数值取整
来源：http://hvo.fktsv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dvd.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://qph.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oes.mhx1999.top

[Q87] JSON 字段做条件
来源：http://kzm.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kbt.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://kyk.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ljw.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://quj.daxiang520.top

[Q89] 判断表是否存在
来源：http://hti.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://grk.dashuyun.cn

[Q90] 生成序号列
来源：http://iso.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rpq.gotoacloud.top

================================================================================
来源：http://zng.shanyushiyangkeji.top

R. Bash 专题
来源：http://wwr.nwbrower.top

================================================================================
来源：http://pis.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://toy.quarkkingdee.top

#!/usr/bin/env bash
来源：http://wiq.guannengcc.top

set -euo pipefail
来源：http://laq.mhx1999.top

[R02] 变量赋值与使用
来源：http://nof.yueranfly.top

name="Tom"; echo "$name"
来源：http://dam.sufxvd.cn

[R03] 只读变量
来源：http://agk.9152youxi.cn

readonly PI=3.14
来源：http://ytj.hammf.cn

[R04] 位置参数
来源：http://dzj.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jam.zhoulong.xyz

[R05] 参数默认值
来源：http://qww.yonumen.top

name="${1:-default}"
来源：http://oml.shzxlz.cn

[R06] 判断命令是否存在
来源：http://lwa.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mvd.gzhubu.top

[R07] if 判断文件
来源：http://lpz.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://evw.tanke756.top

[R08] 数值比较
来源：http://dns.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dbg.xuetiantiany.cn

[R09] 字符串比较
来源：http://ctt.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cgv.yuanzhike.top

[R10] 正则匹配
来源：http://you.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uyx.pengpengdd.cyou

[R11] case 多分支
来源：http://bmf.mhx1999.top

case "$1" in
来源：http://gbm.9152youxi.cn

start) echo "启动" ;;
来源：http://fmt.ivvv.top

stop)  echo "停止" ;;
来源：http://tgj.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://mts.vehdjk.com

esac
来源：http://hxz.dashuyun.cn

[R12] for 遍历文件
来源：http://goi.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://hwx.zhixingplan.top

[R13] for 计数循环
来源：http://uav.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://slu.dianchejie.cn

[R14] C 风格 for
来源：http://xrr.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mec.nwbrower.top

[R15] while 逐行读文件
来源：http://ftf.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wao.ydjk.org.cn

[R16] until 等待条件
来源：http://hhy.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hwk.zhixingplan.top

[R17] 数组定义与取值
来源：http://mpr.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://qzg.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://uud.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kaw.fanxiaobao.xyz

[R19] 数组长度
来源：http://wwb.yvedp.cn

echo "${#arr[@]}"
来源：http://dnt.zhixingplan.top

[R20] 关联数组（字典）
来源：http://scu.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cac.yj20258.top

[R21] 字符串长度
来源：http://jbo.yvedp.cn

echo "${#s}"
来源：http://rnn.hysaishi.cn

[R22] 截取子串
来源：http://bgd.aizwys.cn

echo "${s:0:5}"
来源：http://ksv.zhiwuduotai.top

[R23] 字符串替换
来源：http://ejq.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fic.hnxiangtu.top

[R24] 大小写转换
来源：http://aqa.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gap.ctjpmb.com

[R25] 去后缀 / 去前缀
来源：http://chy.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ccq.zhijiandao.cn

[R26] 命令替换
来源：http://dhv.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://vnb.guannengcc.top

[R27] 算术展开
来源：http://ybb.52xcode.cn

echo $((1 + 2 * 3))
来源：http://vew.52xcode.cn

[R28] 浮点运算
来源：http://hww.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://boq.kuanghao11.cn

[R29] 定义函数
来源：http://afn.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kcg.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://ire.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://yon.sxryk.cn

[R31] 局部变量
来源：http://dkn.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://lxm.shangyingyoupin.top

[R32] 参数个数校验
来源：http://sou.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gnf.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://iye.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vmr.sweek.top

[R34] 退出时清理
来源：http://vzz.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://uie.shuidangran.top

[R35] 后台执行并等待
来源：http://cbh.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://epw.aizwys.cn

[R36] 并发执行多个任务
来源：http://efo.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grq.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://cjw.yanxiufei.cn

files=$(ls -1)
来源：http://ney.zhaomingkeji.xyz

[R38] 管道串联
来源：http://sat.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://wvk.yj20258.top

[R39] 重定向标准输出与错误
来源：http://cko.sjlbkw.cn

cmd > out.log 2>&1
来源：http://bie.fengsongda.top

[R40] 追加写日志
来源：http://hbf.zycfv.cn

echo "log" >> out.log
来源：http://emm.cqqwz.cn

[R41] 丢弃输出
来源：http://szj.sweek.top

cmd >/dev/null 2>&1
来源：http://hoz.zycfv.cn

[R42] 输入重定向
来源：http://oht.9152youxi.cn

wc -l < a.txt
来源：http://nsq.chenlongwang.top

[R43] 按名字查找文件
来源：http://lep.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://owo.yanxiufei.cn

[R44] 按修改时间查找
来源：http://fup.wangdashe.top

find . -mtime -7 -type f
来源：http://yev.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://lyj.52xcode.cn

find . -name "*.tmp" -delete
来源：http://lwp.fzhhl.top

[R46] 递归替换文件内容
来源：http://gcw.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vnj.cqqwz.cn

[R47] sed 单行替换
来源：http://ufw.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tad.ybcxt.top

[R48] awk 取指定列
来源：http://msf.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://gdd.zhiwuduotai.top

[R49] awk 带条件
来源：http://gay.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fjg.tian-w.cn

[R50] awk 求和
来源：http://lrq.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://iom.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://hww.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uzo.yvedp.cn

[R52] 统计行数
来源：http://cto.fzhhl.top

wc -l a.txt
来源：http://lrx.cashguo.top

[R53] 查看文件头与实时尾
来源：http://pgl.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oqq.xinyue.icu

[R54] 比较两个文件
来源：http://ktg.zhixingplan.top

diff a.txt b.txt
来源：http://uov.ctjpmb.com

[R55] 压缩与解压
来源：http://pmd.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zoo.zhongyouzk.top

[R56] 远程拷贝
来源：http://xpn.jiagoushi.top

scp file user@host:/path/
来源：http://uak.chenlongwang.top

[R57] 远程执行命令
来源：http://qyp.cheryme.top

ssh user@host 'uptime'
来源：http://bsg.c1oappe.top

[R58] 下载文件
来源：http://wcw.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oim.tian-w.cn

[R59] 发 POST JSON
来源：http://cgy.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wrx.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://fqm.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nnq.shuidangran.top

[R61] 磁盘占用
来源：http://acz.yfazqb.com

df -h;  du -sh *
来源：http://xmw.birdmap.top

[R62] 找最占空间的文件
来源：http://qsl.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://mdg.tianlin.xyz

[R63] 内存与进程
来源：http://qah.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://vsh.ehwqpu.com

[R64] 结束进程
来源：http://eww.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://lzo.yvedp.cn

[R65] 查看端口占用
来源：http://xyd.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wpo.zhoulong.xyz

[R66] 定时任务
来源：http://jsz.meibo888.top

crontab -e;  crontab -l
来源：http://jyu.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://tjr.hcnkem.com

openssl rand -hex 16
来源：http://ikl.pycfn.com

[R68] 计算文件校验值
来源：http://sxr.yangfankeji.com

sha256sum a.txt;  md5sum a.txt
来源：http://slw.fktsv.cn

[R69] 生成随机密码
来源：http://tto.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://wze.yanxiufei.cn

[R70] 时间戳与互转
来源：http://zdh.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://ojs.fengsongda.top

[R71] 日期格式化
来源：http://rba.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nhd.redwolf501.top

[R72] 等待端口就绪
来源：http://dpi.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yti.aizwys.cn

[R73] 分割大日志
来源：http://tqr.gzhubu.top

split -l 1000 big.log part_
来源：http://hfb.vehdjk.com

[R74] 批量重命名
来源：http://dmz.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://goj.52xcode.cn

[R75] 导出环境变量
来源：http://wyq.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://hlb.cdnleiting.top

[R76] 使用临时文件
来源：http://qmi.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wlo.redwolf501.top

[R77] 读取用户输入
来源：http://mhn.hesvh.cn

read -rp "请输入: " ans
来源：http://qqz.yuanzhike.top

[R78] 交互式菜单
来源：http://zgv.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pcm.fzhhl.top

[R79] 解析命令行选项
来源：http://poo.aibaodan.cn


<!-- 参考信息 -->