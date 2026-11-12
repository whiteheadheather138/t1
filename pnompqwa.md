代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pyq.ctjpmb.com

[Q20] IN 列表
来源：http://wzd.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://buo.mhx1999.top

[Q21] 空值判断
来源：http://ehz.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://vvk.svipenyu.cn

[Q22] 排序
来源：http://kif.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yrv.0kj1m.cn

[Q23] 分页
来源：http://kju.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kyk.gzhubu.top

[Q24] 去重
来源：http://pxf.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://ozb.jianghu66.top

[Q25] 只取前 N 条
来源：http://fso.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bvg.9152youxi.cn

[Q26] 计数
来源：http://vgs.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://qez.bbcook.cn

[Q27] 条件计数
来源：http://rzm.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uns.jinqigufen.top

[Q28] 求和与平均
来源：http://cji.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dft.shuidangran.top

[Q29] 最大最小值
来源：http://taz.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubk.c1oappe.top

[Q30] 分组统计
来源：http://cry.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uew.zhengqikj.top

[Q31] 分组后过滤
来源：http://nif.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gtc.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://bzb.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zku.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://epc.hnqzz.top

[Q33] 多列分组
来源：http://emg.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dqg.hnqzz.top

[Q34] 每组取第一条
来源：http://aai.yj202588.top

SELECT * FROM (
来源：http://ryy.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nfj.xylfe.cn

) t WHERE rn = 1;
来源：http://lky.yongpay.top

[Q35] 内连接
来源：http://udo.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yzm.bbcook.cn

[Q36] 左连接
来源：http://myy.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gnm.jyoumei.cn

[Q37] 右连接
来源：http://nop.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uyh.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vyf.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tmc.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://sjz.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hrb.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jie.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xuk.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oqy.kuanghao11.cn

[Q41] 多表连接
来源：http://edd.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://twr.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://iuw.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://qgo.yj20258.top

[Q42] 连接条件附加过滤
来源：http://ajs.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://ahj.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://leo.ehwqpu.com

[Q43] 标量子查询
来源：http://lwx.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cuu.haohaochexian.top

[Q44] IN 子查询
来源：http://wrd.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xsn.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://bzh.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ste.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hvx.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ndw.bbcook.cn

[Q47] 与平均值比较
来源：http://zwh.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bcm.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://osb.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://joo.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://aex.zhiwuduotai.top

[Q49] 更新单行
来源：http://weo.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hxv.yuxming.cn

[Q50] 批量更新
来源：http://sko.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tta.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://pez.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wvm.zhixingplan.top

[Q52] 删除指定行
来源：http://xqm.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://vvr.haohaochexian.top

[Q53] 按条件删除
来源：http://dpg.guannengcc.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ojs.xziqi.cn

[Q54] 清空表
来源：http://hzx.fengsongda.top

TRUNCATE TABLE logs;
来源：http://vds.havefunace.top

[Q55] 排名（并列占位）
来源：http://yhb.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://urn.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://gzf.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dnm.fengsongda.top

[Q57] 行号
来源：http://cwx.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wej.yj20258.top

[Q58] 累计求和
来源：http://jbe.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ish.jinqigufen.top

[Q59] 分组内累计
来源：http://hxv.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kbg.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://kdr.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mzl.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyl.yuxming.cn

[Q61] 移动平均
来源：http://xih.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyc.daxiang520.top

[Q62] 分组占比
来源：http://wuj.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iut.smart0.xyz

[Q63] 开启事务
来源：http://jvo.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mel.jinqigufen.top

[Q64] 提交事务
来源：http://wtz.gaohongyu789.top

COMMIT;
来源：http://ogw.birdmap.top

[Q65] 回滚事务
来源：http://hkr.fehbvm.com

ROLLBACK;
来源：http://adi.jyoumei.cn

[Q66] 行锁查询
来源：http://neg.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jdv.hcnkem.com

[Q67] 设置隔离级别
来源：http://lde.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sfg.uphjek.com

[Q68] 保存点
来源：http://mal.jinqigufen.top

SAVEPOINT sp1;
来源：http://psj.cdnleiting.top

ROLLBACK TO sp1;
来源：http://bue.mhx1999.top

[Q69] 查看执行计划
来源：http://iww.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bnr.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://hie.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://qin.aibaodan.cn

[Q71] 查看建表语句
来源：http://usl.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://toz.xylfe.cn

[Q72] 查看索引
来源：http://zgs.yj20258.top

SHOW INDEX FROM users;
来源：http://vta.cqqwz.cn

[Q73] 查看表状态
来源：http://wkk.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tso.jinqigufen.top

[Q74] 强制使用索引
来源：http://pry.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qfd.ivvv.top

[Q75] 日期格式化
来源：http://gyw.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vfk.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wyf.tarul.cn

[Q76] 按天统计
来源：http://xza.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nii.aizwys.cn

[Q77] 时间加减
来源：http://uka.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dus.sufxvd.cn

[Q78] 当前时间
来源：http://vxa.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rrc.hammf.cn

[Q79] 字符串拼接
来源：http://znw.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pbq.yj20258.top

[Q80] 字符串截取
来源：http://jwv.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lkm.pycfn.com

[Q81] 字符串替换
来源：http://psv.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://muj.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://cii.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqv.zdbjq.cn

[Q83] 大小写转换
来源：http://pgv.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dwy.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://zfp.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://ajt.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://iqd.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gui.meibo888.top

[Q86] 读取 JSON 字段
来源：http://uni.sweek.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yjn.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://wgs.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pud.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://pbo.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://emg.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yqq.hcnkem.com

[Q89] 判断表是否存在
来源：http://tls.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://exu.xuetiantiany.cn

[Q90] 生成序号列
来源：http://mhf.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://moj.vqdsnc.cn

================================================================================
来源：http://dww.pycfn.com

R. Bash 专题
来源：http://hgi.cqqwz.cn

================================================================================
来源：http://wkf.xuanzx.com

[R01] shebang 与严格模式
来源：http://pvg.316326.xyz

#!/usr/bin/env bash
来源：http://zts.daxiang520.top

set -euo pipefail
来源：http://ddo.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://wlk.havefunace.top

name="Tom"; echo "$name"
来源：http://nga.chenzaomai.com

[R03] 只读变量
来源：http://sxo.zhiwuduotai.top

readonly PI=3.14
来源：http://ghf.jqgfzy.top

[R04] 位置参数
来源：http://lyr.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://anl.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://bcg.aibaodan.cn

name="${1:-default}"
来源：http://jkz.haohaochexian.top

[R06] 判断命令是否存在
来源：http://eim.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fjl.zhengqikj.top

[R07] if 判断文件
来源：http://jvs.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tnc.c1oappe.top

[R08] 数值比较
来源：http://dqx.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://awc.bbcook.cn

[R09] 字符串比较
来源：http://rht.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nhs.dashuyun.cn

[R10] 正则匹配
来源：http://ice.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vip.yj202588.top

[R11] case 多分支
来源：http://kiy.andypj.xyz

case "$1" in
来源：http://bkj.9152youxi.cn

start) echo "启动" ;;
来源：http://oux.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://sef.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://sku.quarkkingdee.top

esac
来源：http://hlp.ehwqpu.com

[R12] for 遍历文件
来源：http://vks.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://qjj.jinghuilouyu.cn

[R13] for 计数循环
来源：http://mxx.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://wfq.ivvv.top

[R14] C 风格 for
来源：http://pry.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fgq.hcnkem.com

[R15] while 逐行读文件
来源：http://rbr.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iwd.zhixingplan.top

[R16] until 等待条件
来源：http://vme.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://btt.xziqi.cn

[R17] 数组定义与取值
来源：http://yfe.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://xfq.dashuyun.cn

[R18] 遍历数组
来源：http://gli.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aex.hongshengwenyu.top

[R19] 数组长度
来源：http://ppa.yj20258.top

echo "${#arr[@]}"
来源：http://izb.tian-w.cn

[R20] 关联数组（字典）
来源：http://lck.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aul.chenjidiqi.icu

[R21] 字符串长度
来源：http://lkm.aizwys.cn

echo "${#s}"
来源：http://hrh.ivvv.top

[R22] 截取子串
来源：http://gbg.gaohongyu789.top

echo "${s:0:5}"
来源：http://ofy.52xcode.cn

[R23] 字符串替换
来源：http://goc.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rzd.gotoacloud.top

[R24] 大小写转换
来源：http://bzc.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://kgh.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://dch.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ayd.gaohongyu789.top

[R26] 命令替换
来源：http://wwe.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://rid.haohaochexian.top

[R27] 算术展开
来源：http://kcw.sysykeji.top

echo $((1 + 2 * 3))
来源：http://sod.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://xhi.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://oys.bjfxy.top

[R29] 定义函数
来源：http://hro.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xme.yuanzhike.top

[R30] 函数返回状态码
来源：http://kix.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://abi.kuanghao11.cn

[R31] 局部变量
来源：http://bql.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://ajr.smart0.xyz

[R32] 参数个数校验
来源：http://kka.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abj.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://ssq.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://unh.yongpay.top

[R34] 退出时清理
来源：http://oav.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ezf.pycfn.com

[R35] 后台执行并等待
来源：http://bay.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jci.hcnkem.com

[R36] 并发执行多个任务
来源：http://bsw.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eim.gotoacloud.top

[R37] 把输出赋给变量
来源：http://ehq.zycfv.cn

files=$(ls -1)
来源：http://jyd.sufxvd.cn

[R38] 管道串联
来源：http://eag.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://grg.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://kmi.hcnkem.com

cmd > out.log 2>&1
来源：http://rtr.dashuyun.cn

[R40] 追加写日志
来源：http://yrp.ydjk.org.cn

echo "log" >> out.log
来源：http://tbc.zhijiandao.cn

[R41] 丢弃输出
来源：http://qmm.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://mvl.yvedp.cn

[R42] 输入重定向
来源：http://cww.tian-w.cn

wc -l < a.txt
来源：http://sjx.mhx1999.top

[R43] 按名字查找文件
来源：http://qal.dianchejie.cn

find . -name "*.log" -type f
来源：http://fuj.xuanzx.com

[R44] 按修改时间查找
来源：http://kub.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://lnq.haohaochexian.top

[R45] 批量删除
来源：http://tek.xylfe.cn

find . -name "*.tmp" -delete
来源：http://kdr.mhx1999.top

[R46] 递归替换文件内容
来源：http://opn.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ztk.hywenlv.cn

[R47] sed 单行替换
来源：http://lmx.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lwh.sxryk.cn

[R48] awk 取指定列
来源：http://dws.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://ojf.jiagoushi.top

[R49] awk 带条件
来源：http://udz.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://plt.jinghuilouyu.cn

[R50] awk 求和
来源：http://cgs.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://rzt.zdbjq.cn

[R51] 排序去重取前几
来源：http://byl.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gsx.316326.xyz

[R52] 统计行数
来源：http://lkh.jinyuanbaomall.cn

wc -l a.txt
来源：http://gup.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://hzz.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gkj.gotoacloud.top

[R54] 比较两个文件
来源：http://hwa.sjlbkw.cn

diff a.txt b.txt
来源：http://ouu.fzhhl.top

[R55] 压缩与解压
来源：http://ent.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nuj.yuxming.cn

[R56] 远程拷贝
来源：http://gaa.ydjk.org.cn

scp file user@host:/path/
来源：http://inv.gotoacloud.top

[R57] 远程执行命令
来源：http://ljy.zhixingplan.top

ssh user@host 'uptime'
来源：http://acl.gzhubu.top

[R58] 下载文件
来源：http://gyh.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gpo.yj20258888.top

[R59] 发 POST JSON
来源：http://mpx.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jva.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://hmv.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aiv.hongshengwenyu.top

[R61] 磁盘占用
来源：http://izl.9152youxi.cn

df -h;  du -sh *
来源：http://gpz.9152youxi.cn

[R62] 找最占空间的文件
来源：http://hsp.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://dnz.fehbvm.com

[R63] 内存与进程
来源：http://mnk.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://wsg.yfazqb.com

[R64] 结束进程
来源：http://xda.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://vxm.jlsjyb.cn

[R65] 查看端口占用
来源：http://tnm.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eue.zhoulong.xyz

[R66] 定时任务
来源：http://eaf.jlsjyb.cn

crontab -e;  crontab -l
来源：http://mcv.tanke756.top

[R67] 生成随机十六进制串
来源：http://fmr.xziqi.cn

openssl rand -hex 16
来源：http://zip.yonumen.top

[R68] 计算文件校验值
来源：http://cmd.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ofv.redwolf501.top

[R69] 生成随机密码
来源：http://qlz.jqgfzy.top


<!-- 参考信息 -->