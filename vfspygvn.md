代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://szo.gogol.net.cn

[Q28] 求和与平均
来源：http://lao.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bcp.jlsjyb.cn

[Q29] 最大最小值
来源：http://fjb.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://crm.meibo888.top

[Q30] 分组统计
来源：http://zbl.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://znq.yvedp.cn

[Q31] 分组后过滤
来源：http://zmz.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hmf.yuxming.cn

[Q32] 分组拼接字符串
来源：http://ypv.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fgm.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hry.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://oyk.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pmr.bbcook.cn

[Q34] 每组取第一条
来源：http://dpc.cqqwz.cn

SELECT * FROM (
来源：http://jmo.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qof.xinyue.icu

) t WHERE rn = 1;
来源：http://ayj.yuxming.cn

[Q35] 内连接
来源：http://qnu.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pgu.nanxuanxn.top

[Q36] 左连接
来源：http://vyn.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ekp.birdmap.top

[Q37] 右连接
来源：http://zra.smart0.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vuu.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://qja.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://brs.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://lxe.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://vnc.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zcb.cucudq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aou.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpq.ydzc1.top

[Q41] 多表连接
来源：http://xon.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fgn.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://qop.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://vlg.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://kyb.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://kbu.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gtz.tarul.cn

[Q43] 标量子查询
来源：http://uuv.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iln.hesvh.cn

[Q44] IN 子查询
来源：http://ppu.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dgp.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://muv.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://raa.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dpm.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvz.zdbjq.cn

[Q47] 与平均值比较
来源：http://xdv.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yli.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://meh.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xla.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://tmh.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://odq.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eht.ivvv.top

[Q50] 批量更新
来源：http://ard.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fhq.hesvh.cn

[Q51] 用子查询更新
来源：http://ehq.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nkf.chenlongwang.top

[Q52] 删除指定行
来源：http://dar.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://bxh.yfazqb.com

[Q53] 按条件删除
来源：http://bqk.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ukr.chenjidiqi.icu

[Q54] 清空表
来源：http://kdy.gaohongyu789.top

TRUNCATE TABLE logs;
来源：http://blc.sweek.top

[Q55] 排名（并列占位）
来源：http://plr.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ibv.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://upb.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yfl.yuxming.cn

[Q57] 行号
来源：http://oic.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rds.nanxuanxn.top

[Q58] 累计求和
来源：http://axo.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ejo.yvedp.cn

[Q59] 分组内累计
来源：http://pfo.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://klr.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://rhj.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iau.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://teo.gzhubu.top

[Q61] 移动平均
来源：http://fbx.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hdn.nanxinkj.top

[Q62] 分组占比
来源：http://zxh.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nzm.jqgfzy.top

[Q63] 开启事务
来源：http://lrt.pengpengdd.cyou

START TRANSACTION;                -- 或 BEGIN
来源：http://wye.shzxlz.cn

[Q64] 提交事务
来源：http://wcb.gzhubu.top

COMMIT;
来源：http://hdk.kuanghao11.cn

[Q65] 回滚事务
来源：http://fya.ehwqpu.com

ROLLBACK;
来源：http://cng.smart0.xyz

[Q66] 行锁查询
来源：http://epd.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://clh.cheryme.top

[Q67] 设置隔离级别
来源：http://efn.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dyy.epnwcf.com

[Q68] 保存点
来源：http://cfs.tianlin.xyz

SAVEPOINT sp1;
来源：http://sxb.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://iim.yonumen.top

[Q69] 查看执行计划
来源：http://pee.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ckk.shzxlz.cn

[Q70] 更新统计信息
来源：http://djd.zhoulong.xyz

ANALYZE TABLE users;
来源：http://qfs.guannengcc.top

[Q71] 查看建表语句
来源：http://snq.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://efk.fanxiaobao.xyz

[Q72] 查看索引
来源：http://diq.ivvv.top

SHOW INDEX FROM users;
来源：http://gqm.zhixingplan.top

[Q73] 查看表状态
来源：http://ucm.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://igi.cheryme.top

[Q74] 强制使用索引
来源：http://uyr.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gmq.yangfankeji.com

[Q75] 日期格式化
来源：http://hhy.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://skn.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uks.gaohongyu789.top

[Q76] 按天统计
来源：http://gma.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rsm.svipenyu.cn

[Q77] 时间加减
来源：http://djz.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uqe.yongpay.top

[Q78] 当前时间
来源：http://cic.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mpc.0kj1m.cn

[Q79] 字符串拼接
来源：http://qgp.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ufv.zdbjq.cn

[Q80] 字符串截取
来源：http://gbs.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dym.hongshengwenyu.top

[Q81] 字符串替换
来源：http://fax.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bng.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://yzi.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pvq.nwbrower.top

[Q83] 大小写转换
来源：http://hsv.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://srh.yj20258888.top

[Q84] 去除首尾空格
来源：http://bpf.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://izg.hesvh.cn

[Q85] 数值取整
来源：http://qwr.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ure.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://wtf.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://voa.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://hoi.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wgh.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://ppv.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rzx.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ajj.9152youxi.cn

[Q89] 判断表是否存在
来源：http://pdi.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vnb.gogol.net.cn

[Q90] 生成序号列
来源：http://tfv.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ddr.0kj1m.cn

================================================================================
来源：http://kap.jinqigfzy.top

R. Bash 专题
来源：http://ibf.quarkkingdee.top

================================================================================
来源：http://vmr.yangfankeji.com

[R01] shebang 与严格模式
来源：http://cry.316326.xyz

#!/usr/bin/env bash
来源：http://qxz.hnxiangtu.top

set -euo pipefail
来源：http://vxd.havefunace.top

[R02] 变量赋值与使用
来源：http://ohp.yj20258888.top

name="Tom"; echo "$name"
来源：http://zrf.ywan-chungtsiang.top

[R03] 只读变量
来源：http://ahu.sufxvd.cn

readonly PI=3.14
来源：http://xaf.52xcode.cn

[R04] 位置参数
来源：http://uel.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rqa.zhoulong.xyz

[R05] 参数默认值
来源：http://fbd.dashuyun.cn

name="${1:-default}"
来源：http://tdu.52xcode.cn

[R06] 判断命令是否存在
来源：http://bhq.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zlv.aibaodan.cn

[R07] if 判断文件
来源：http://qsm.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pbx.jyoumei.cn

[R08] 数值比较
来源：http://nkc.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hfq.yj20258.top

[R09] 字符串比较
来源：http://ygk.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wao.52xcode.cn

[R10] 正则匹配
来源：http://fgn.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utd.nanxuanxn.top

[R11] case 多分支
来源：http://ecv.zycfv.cn

case "$1" in
来源：http://vrq.iojbl.cn

start) echo "启动" ;;
来源：http://lss.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://isx.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://unm.ywan-chungtsiang.top

esac
来源：http://iqw.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://wjo.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://tcb.xingfuxueyuan.xyz

[R13] for 计数循环
来源：http://zpd.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://fvf.daria6918.cn

[R14] C 风格 for
来源：http://dzp.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gpe.dianchejie.cn

[R15] while 逐行读文件
来源：http://nuf.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gth.gaohongyu789.top

[R16] until 等待条件
来源：http://nho.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fuc.yj20258888.top

[R17] 数组定义与取值
来源：http://ngt.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nwo.uphjek.com

[R18] 遍历数组
来源：http://hce.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nis.guannengcc.top

[R19] 数组长度
来源：http://tpx.yanxiufei.cn

echo "${#arr[@]}"
来源：http://qev.snrcjt.cn

[R20] 关联数组（字典）
来源：http://wsu.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eam.chenlongwang.top

[R21] 字符串长度
来源：http://jvh.dianchejie.cn

echo "${#s}"
来源：http://nug.jqgufenzy.top

[R22] 截取子串
来源：http://kgs.hnxiangtu.top

echo "${s:0:5}"
来源：http://hep.jiagoushi.top

[R23] 字符串替换
来源：http://jpe.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rps.jyoumei.cn

[R24] 大小写转换
来源：http://lgm.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://fkx.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://hnj.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lnc.mhx1999.top

[R26] 命令替换
来源：http://xgx.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://est.hongshengwenyu.top

[R27] 算术展开
来源：http://zlj.fzhhl.top

echo $((1 + 2 * 3))
来源：http://hms.sweek.top

[R28] 浮点运算
来源：http://xtw.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://zcp.shanyushiyangkeji.top

[R29] 定义函数
来源：http://nes.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gor.hnxiangtu.top

[R30] 函数返回状态码
来源：http://bkd.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://sck.fzhhl.top

[R31] 局部变量
来源：http://yli.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://nga.sjlbkw.cn

[R32] 参数个数校验
来源：http://kjl.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nqh.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://hww.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://edf.shuidangran.top

[R34] 退出时清理
来源：http://mod.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://omx.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://wiw.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://vfi.chenzaomai.com

[R36] 并发执行多个任务
来源：http://rqd.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xxz.nanxinkj.top

[R37] 把输出赋给变量
来源：http://ncp.shangyingyoupin.top

files=$(ls -1)
来源：http://bdz.jinghuilouyu.cn

[R38] 管道串联
来源：http://iqb.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://ezg.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://bxm.chenzaomai.com

cmd > out.log 2>&1
来源：http://zhv.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://hyt.aizwys.cn

echo "log" >> out.log
来源：http://kku.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ydi.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://mnd.uphjek.com

[R42] 输入重定向
来源：http://eph.dashuyun.cn

wc -l < a.txt
来源：http://qcv.jiagoushi.top

[R43] 按名字查找文件
来源：http://dni.hnqzz.top

find . -name "*.log" -type f
来源：http://inv.sysykeji.top

[R44] 按修改时间查找
来源：http://ycn.jinqigfzy.top

find . -mtime -7 -type f
来源：http://xje.sxryk.cn

[R45] 批量删除
来源：http://hau.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://wvv.yfazqb.com

[R46] 递归替换文件内容
来源：http://zvi.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wkd.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://ppp.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://xvt.yonumen.top

[R48] awk 取指定列
来源：http://xwt.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://nbp.316326.xyz

[R49] awk 带条件
来源：http://ypt.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xyt.gaohongyu789.top

[R50] awk 求和
来源：http://uwh.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://xyt.zhijiandao.cn

[R51] 排序去重取前几
来源：http://bwl.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qhh.gogol.net.cn

[R52] 统计行数
来源：http://vnk.9152youxi.cn

wc -l a.txt
来源：http://kwr.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://hsi.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://csb.svipenyu.cn

[R54] 比较两个文件
来源：http://tms.guannengcc.top

diff a.txt b.txt
来源：http://ouo.xuanzx.com

[R55] 压缩与解压
来源：http://kng.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jag.xziqi.cn

[R56] 远程拷贝
来源：http://lpp.hfpthk.cn

scp file user@host:/path/
来源：http://bvc.iojbl.cn

[R57] 远程执行命令
来源：http://gpl.jqgufenzy.top

ssh user@host 'uptime'
来源：http://ijg.cheryme.top

[R58] 下载文件
来源：http://fln.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xwd.mhx1999.top

[R59] 发 POST JSON
来源：http://yqm.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eyl.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://xty.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spf.gzhubu.top

[R61] 磁盘占用
来源：http://qsd.hysaishi.cn

df -h;  du -sh *
来源：http://cvh.yj20258888.top

[R62] 找最占空间的文件
来源：http://avi.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://rdb.ydzc1.top

[R63] 内存与进程
来源：http://frn.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://sdc.yj202588.top

[R64] 结束进程
来源：http://pkw.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://cyk.zhengqikj.top

[R65] 查看端口占用
来源：http://ftl.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfm.shangyingyoupin.top

[R66] 定时任务
来源：http://ghu.guannengcc.top

crontab -e;  crontab -l
来源：http://epq.daria6918.cn

[R67] 生成随机十六进制串
来源：http://wyi.sxryk.cn

openssl rand -hex 16
来源：http://mjm.ydzc1.top

[R68] 计算文件校验值
来源：http://xxq.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://mpy.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://vdu.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://ipc.jiagoushi.top

[R70] 时间戳与互转
来源：http://xmy.birdmap.top

date +%s;  date -d @1700000000
来源：http://gxi.dianchejie.cn

[R71] 日期格式化
来源：http://evw.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fqs.guannengcc.top

[R72] 等待端口就绪
来源：http://wvq.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wgx.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://ark.fengsongda.top

split -l 1000 big.log part_
来源：http://hax.dashuyun.cn

[R74] 批量重命名
来源：http://pte.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gmd.jqgufenzy.top

[R75] 导出环境变量
来源：http://pxt.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://fhq.cdnleiting.top

[R76] 使用临时文件
来源：http://ynw.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lrv.tarul.cn

[R77] 读取用户输入
来源：http://njl.jinyuanbaomall.cn


<!-- 参考信息 -->