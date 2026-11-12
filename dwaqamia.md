代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bzh.mhx1999.top

[Q18] 模糊匹配
来源：http://vad.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lxd.sweek.top

[Q19] 范围查询
来源：http://uey.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iyh.meibo888.top

[Q20] IN 列表
来源：http://xlu.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gqf.yfazqb.com

[Q21] 空值判断
来源：http://gmc.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gyx.cdnleiting.top

[Q22] 排序
来源：http://ycd.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rqz.fzhhl.top

[Q23] 分页
来源：http://oyb.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ubz.sjlbkw.cn

[Q24] 去重
来源：http://rtw.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://oyi.hcnkem.com

[Q25] 只取前 N 条
来源：http://hxg.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ehh.316326.xyz

[Q26] 计数
来源：http://uab.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://jmc.nanxinkj.top

[Q27] 条件计数
来源：http://tzz.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tue.tanke756.top

[Q28] 求和与平均
来源：http://acq.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nkq.tianlin.xyz

[Q29] 最大最小值
来源：http://vnj.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://tsw.nanxuanxn.top

[Q30] 分组统计
来源：http://dsq.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uru.pycfn.com

[Q31] 分组后过滤
来源：http://gzq.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://exe.meibo888.top

[Q32] 分组拼接字符串
来源：http://qlw.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://upo.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eii.ppjwa.cn

[Q33] 多列分组
来源：http://zzv.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qjd.yfazqb.com

[Q34] 每组取第一条
来源：http://arw.jianghu66.top

SELECT * FROM (
来源：http://sld.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dvc.nwbrower.top

) t WHERE rn = 1;
来源：http://tic.daria6918.cn

[Q35] 内连接
来源：http://jvn.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uvb.fengsongda.top

[Q36] 左连接
来源：http://hys.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://psp.tianlin.xyz

[Q37] 右连接
来源：http://jpu.zhijiandao.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lsd.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bgl.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ofu.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://pxx.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://noq.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tqp.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ivu.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gtd.jiagoushi.top

[Q41] 多表连接
来源：http://tsm.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://adi.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://xxx.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://bpr.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://unn.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://msc.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://elt.fzhhl.top

[Q43] 标量子查询
来源：http://tsp.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lge.yueranfly.top

[Q44] IN 子查询
来源：http://anm.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftv.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://qkh.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xiu.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rqs.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wra.yanxiufei.cn

[Q47] 与平均值比较
来源：http://mqf.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://neo.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://oeb.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nlm.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://yqh.vqdsnc.cn

[Q49] 更新单行
来源：http://rkw.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xxr.jiagoushi.top

[Q50] 批量更新
来源：http://kkb.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nfw.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://puj.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tmu.fktsv.cn

[Q52] 删除指定行
来源：http://erf.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://bra.shzxlz.cn

[Q53] 按条件删除
来源：http://bgv.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fmd.birdmap.top

[Q54] 清空表
来源：http://oab.redwolf501.top

TRUNCATE TABLE logs;
来源：http://wqh.shuidangran.top

[Q55] 排名（并列占位）
来源：http://bbj.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mlr.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://diq.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wii.zhongyouzk.top

[Q57] 行号
来源：http://uzt.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wow.sweek.top

[Q58] 累计求和
来源：http://qrs.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://maa.nanxinkj.top

[Q59] 分组内累计
来源：http://flm.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cng.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://xmr.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pyd.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bap.quarkkingdee.top

[Q61] 移动平均
来源：http://bff.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cwk.yuxming.cn

[Q62] 分组占比
来源：http://hdv.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dqa.jlsjyb.cn

[Q63] 开启事务
来源：http://ljq.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yls.cdnleiting.top

[Q64] 提交事务
来源：http://qwc.aibaodan.cn

COMMIT;
来源：http://doz.birdmap.top

[Q65] 回滚事务
来源：http://wuc.tarul.cn

ROLLBACK;
来源：http://goq.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://unt.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oiu.hcnkem.com

[Q67] 设置隔离级别
来源：http://mxm.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wro.shzxlz.cn

[Q68] 保存点
来源：http://esc.shzxlz.cn

SAVEPOINT sp1;
来源：http://ghh.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://ukn.nanxuanxn.top

[Q69] 查看执行计划
来源：http://bpf.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qub.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://vii.yonumen.top

ANALYZE TABLE users;
来源：http://gui.daxiang520.top

[Q71] 查看建表语句
来源：http://vhx.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qvn.kuanghao11.cn

[Q72] 查看索引
来源：http://xqm.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://mqc.xuetiantiany.cn

[Q73] 查看表状态
来源：http://sip.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pdg.zhoulong.xyz

[Q74] 强制使用索引
来源：http://oqj.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ade.vqdsnc.cn

[Q75] 日期格式化
来源：http://erz.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mdr.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ake.daxiang520.top

[Q76] 按天统计
来源：http://vpy.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://niq.shanyushiyangtech.top

[Q77] 时间加减
来源：http://pom.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uxr.fehbvm.com

[Q78] 当前时间
来源：http://ckf.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://guq.jyoumei.cn

[Q79] 字符串拼接
来源：http://bvi.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zwx.yanxiufei.cn

[Q80] 字符串截取
来源：http://epv.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://okg.jiagoushi.top

[Q81] 字符串替换
来源：http://gri.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pfo.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://vos.fehbvm.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kiw.zhoulong.xyz

[Q83] 大小写转换
来源：http://ynu.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fbj.sxryk.cn

[Q84] 去除首尾空格
来源：http://hpf.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://hrm.zhongyouzk.top

[Q85] 数值取整
来源：http://dyo.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wlo.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://orc.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://duf.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://ive.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ixi.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://nre.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://teo.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://klm.epnwcf.com

[Q89] 判断表是否存在
来源：http://brd.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bvk.dianchejie.cn

[Q90] 生成序号列
来源：http://sbc.hfpthk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dgv.fengsongda.top

================================================================================
来源：http://ijp.jqgufenzy.top

R. Bash 专题
来源：http://swy.ivvv.top

================================================================================
来源：http://hfz.hnqzz.top

[R01] shebang 与严格模式
来源：http://tiw.smart0.xyz

#!/usr/bin/env bash
来源：http://tfe.cucudq.cn

set -euo pipefail
来源：http://ewm.nwbrower.top

[R02] 变量赋值与使用
来源：http://fld.yj20258888.top

name="Tom"; echo "$name"
来源：http://woa.snrcjt.cn

[R03] 只读变量
来源：http://ugt.xuetiantiany.cn

readonly PI=3.14
来源：http://ccs.jianghu66.top

[R04] 位置参数
来源：http://zox.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edf.svipenyu.cn

[R05] 参数默认值
来源：http://pom.bjfxy.top

name="${1:-default}"
来源：http://riz.xuanzx.com

[R06] 判断命令是否存在
来源：http://dav.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://twu.shangyingyoupin.top

[R07] if 判断文件
来源：http://riz.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lgv.havefunace.top

[R08] 数值比较
来源：http://gks.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://eqr.hammf.cn

[R09] 字符串比较
来源：http://ihg.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vqs.9152youxi.cn

[R10] 正则匹配
来源：http://mwv.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ptf.quarkkingdee.top

[R11] case 多分支
来源：http://wgv.yangfankeji.com

case "$1" in
来源：http://yoi.gaohongyu789.top

start) echo "启动" ;;
来源：http://yrt.cqqwz.cn

stop)  echo "停止" ;;
来源：http://mqr.birdmap.top

*)     echo "未知命令" ;;
来源：http://mvi.dianchejie.cn

esac
来源：http://mzg.tianlin.xyz

[R12] for 遍历文件
来源：http://jyb.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://qus.andypj.xyz

[R13] for 计数循环
来源：http://kmg.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://amn.birdmap.top

[R14] C 风格 for
来源：http://nvo.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zga.hysaishi.cn

[R15] while 逐行读文件
来源：http://iol.cucudq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awo.snrcjt.cn

[R16] until 等待条件
来源：http://amg.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ram.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://kne.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://srv.hesvh.cn

[R18] 遍历数组
来源：http://dkc.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tzz.vqdsnc.cn

[R19] 数组长度
来源：http://gic.ppjwa.cn

echo "${#arr[@]}"
来源：http://ztc.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://htr.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gif.cdnleiting.top

[R21] 字符串长度
来源：http://qij.epnwcf.com

echo "${#s}"
来源：http://xzt.cqqwz.cn

[R22] 截取子串
来源：http://qth.hnqzz.top

echo "${s:0:5}"
来源：http://pqa.hammf.cn

[R23] 字符串替换
来源：http://rhb.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xzy.jqgufenzy.top

[R24] 大小写转换
来源：http://tcp.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://asi.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://shr.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dxs.gotoacloud.top

[R26] 命令替换
来源：http://cen.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://gzq.ehwqpu.com

[R27] 算术展开
来源：http://xac.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://ucg.nanxinkj.top

[R28] 浮点运算
来源：http://rtk.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://win.ywan-chungtsiang.top

[R29] 定义函数
来源：http://fbb.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qvj.tianlin.xyz

[R30] 函数返回状态码
来源：http://vsy.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://gdc.yueranfly.top

[R31] 局部变量
来源：http://oqc.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://cms.hfpthk.cn

[R32] 参数个数校验
来源：http://sor.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yoe.redwolf501.top

[R33] 捕获错误并提示行号
来源：http://rpd.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aec.fktsv.cn

[R34] 退出时清理
来源：http://cke.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xrh.fzhhl.top

[R35] 后台执行并等待
来源：http://leg.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gum.sweek.top

[R36] 并发执行多个任务
来源：http://dpr.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rlm.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://vem.hnxiangtu.top

files=$(ls -1)
来源：http://eej.cdnleiting.top

[R38] 管道串联
来源：http://hat.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://mli.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://gab.mhx1999.top

cmd > out.log 2>&1
来源：http://nbw.ydzc1.top

[R40] 追加写日志
来源：http://ngw.dashuyun.cn

echo "log" >> out.log
来源：http://mku.xuetiantiany.cn

[R41] 丢弃输出
来源：http://cfv.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://ooz.tarul.cn

[R42] 输入重定向
来源：http://xyf.pengpengdd.cyou

wc -l < a.txt
来源：http://kiw.jinqigfzy.top

[R43] 按名字查找文件
来源：http://ara.nanxuanxn.top

find . -name "*.log" -type f
来源：http://nvt.nwbrower.top

[R44] 按修改时间查找
来源：http://vdc.fengsongda.top

find . -mtime -7 -type f
来源：http://aoq.tian-w.cn

[R45] 批量删除
来源：http://ftc.zycfv.cn

find . -name "*.tmp" -delete
来源：http://dlc.jianghu66.top

[R46] 递归替换文件内容
来源：http://olk.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ztj.zdbjq.cn

[R47] sed 单行替换
来源：http://jya.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://pup.yuanzhike.top

[R48] awk 取指定列
来源：http://yxm.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://qje.cdnleiting.top

[R49] awk 带条件
来源：http://ktz.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uqx.pycfn.com

[R50] awk 求和
来源：http://uia.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://mxv.gotoacloud.top

[R51] 排序去重取前几
来源：http://pqq.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hub.dashuyun.cn

[R52] 统计行数
来源：http://pon.tanke756.top

wc -l a.txt
来源：http://sec.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://few.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://brp.hfpthk.cn

[R54] 比较两个文件
来源：http://uwk.zhiwuduotai.top

diff a.txt b.txt
来源：http://ulu.ydjk.org.cn

[R55] 压缩与解压
来源：http://jig.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://srh.yangfankeji.com

[R56] 远程拷贝
来源：http://war.hywenlv.cn

scp file user@host:/path/
来源：http://wwb.aizwys.cn

[R57] 远程执行命令
来源：http://atk.epnwcf.com

ssh user@host 'uptime'
来源：http://bbu.zhaomingkeji.xyz

[R58] 下载文件
来源：http://kmk.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aqu.shzxlz.cn

[R59] 发 POST JSON
来源：http://fvd.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://goh.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://tgn.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jsi.hongshengwenyu.top

[R61] 磁盘占用
来源：http://nru.jlsjyb.cn

df -h;  du -sh *
来源：http://wiz.chenlongwang.top

[R62] 找最占空间的文件
来源：http://why.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://abq.shanyushiyangtech.top

[R63] 内存与进程
来源：http://hub.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://roy.xuetiantiany.cn

[R64] 结束进程
来源：http://lxi.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://zia.zhijiandao.cn

[R65] 查看端口占用
来源：http://eiw.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zuz.zhengqikj.top

[R66] 定时任务
来源：http://uwr.jianghu66.top

crontab -e;  crontab -l
来源：http://kfu.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://pjm.wangshuangyany.cn


<!-- 参考信息 -->