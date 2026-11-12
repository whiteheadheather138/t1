代发 wailian999

SELECT * FROM users;
来源：http://jmq.uphjek.com

[Q16] 查询指定列
来源：http://uow.svipenyu.cn

SELECT id, name FROM users;
来源：http://cnx.fehbvm.com

[Q17] 条件查询
来源：http://kvo.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kvz.jqgufenzy.top

[Q18] 模糊匹配
来源：http://dfm.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pcb.ybcxt.top

[Q19] 范围查询
来源：http://stb.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qba.cucudq.cn

[Q20] IN 列表
来源：http://ahy.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nad.fehbvm.com

[Q21] 空值判断
来源：http://zsn.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aad.hongshengwenyu.top

[Q22] 排序
来源：http://ort.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gbu.cashguo.top

[Q23] 分页
来源：http://yzr.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qqo.wangshuangyany.cn

[Q24] 去重
来源：http://fhi.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://kpt.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://hbh.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yaa.hammf.cn

[Q26] 计数
来源：http://egz.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://umi.epnwcf.com

[Q27] 条件计数
来源：http://mbu.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rqu.316326.xyz

[Q28] 求和与平均
来源：http://mda.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bwf.c1oappe.top

[Q29] 最大最小值
来源：http://mpw.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://utw.daria6918.cn

[Q30] 分组统计
来源：http://clm.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gko.sxryk.cn

[Q31] 分组后过滤
来源：http://xal.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qvw.ydzc1.top

[Q32] 分组拼接字符串
来源：http://zfx.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dst.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tos.ehwqpu.com

[Q33] 多列分组
来源：http://ccq.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gjj.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://kuh.zhoulong.xyz

SELECT * FROM (
来源：http://pcr.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cuy.gaohongyu789.top

) t WHERE rn = 1;
来源：http://ntq.yuanzhike.top

[Q35] 内连接
来源：http://bca.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvt.jqgfzy.top

[Q36] 左连接
来源：http://iha.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://osp.svipenyu.cn

[Q37] 右连接
来源：http://gcz.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://quz.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://rdv.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://anp.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://aqu.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pxq.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://khz.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hye.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://emh.c1oappe.top

[Q41] 多表连接
来源：http://hah.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iyt.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://hmy.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://uhm.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://bmu.xylfe.cn

SELECT u.name, o.amount FROM users u
来源：http://cjr.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wdw.yonumen.top

[Q43] 标量子查询
来源：http://csd.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nsi.zhiwuduotai.top

[Q44] IN 子查询
来源：http://eom.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qyl.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://mqc.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gnf.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tyr.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xnk.fehbvm.com

[Q47] 与平均值比较
来源：http://zyb.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iqu.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://mef.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gnt.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://etq.wangshuangyany.cn

[Q49] 更新单行
来源：http://fac.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wvo.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://yzb.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://but.yangfankeji.com

[Q51] 用子查询更新
来源：http://bsl.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gzv.sysykeji.top

[Q52] 删除指定行
来源：http://xen.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://ezo.tarul.cn

[Q53] 按条件删除
来源：http://fsz.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gpr.shanyushiyangkeji.top

[Q54] 清空表
来源：http://whx.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://ljp.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://rik.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eho.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://ljx.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gzs.jinqigufen.top

[Q57] 行号
来源：http://ilf.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rdx.shanyushiyangtech.top

[Q58] 累计求和
来源：http://cuz.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qab.epnwcf.com

[Q59] 分组内累计
来源：http://fah.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eyv.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://xlz.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://apn.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://axv.tanke756.top

[Q61] 移动平均
来源：http://vfg.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pqo.guowangkeji.top

[Q62] 分组占比
来源：http://aoh.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mti.sysykeji.top

[Q63] 开启事务
来源：http://kip.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qgv.yj20258.top

[Q64] 提交事务
来源：http://wle.pycfn.com

COMMIT;
来源：http://zcs.guannengcc.top

[Q65] 回滚事务
来源：http://rhb.gogol.net.cn

ROLLBACK;
来源：http://toc.sweek.top

[Q66] 行锁查询
来源：http://dty.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kej.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://tda.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dlw.zhijiandao.cn

[Q68] 保存点
来源：http://usf.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://rkk.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://oer.gaohongyu789.top

[Q69] 查看执行计划
来源：http://qbj.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://liy.yueranfly.top

[Q70] 更新统计信息
来源：http://vrr.epnwcf.com

ANALYZE TABLE users;
来源：http://czi.hfpthk.cn

[Q71] 查看建表语句
来源：http://kbg.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://awn.cheryme.top

[Q72] 查看索引
来源：http://fgs.bjfxy.top

SHOW INDEX FROM users;
来源：http://vdf.yonumen.top

[Q73] 查看表状态
来源：http://qrz.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nwg.snrcjt.cn

[Q74] 强制使用索引
来源：http://yil.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qmp.chenjidiqi.icu

[Q75] 日期格式化
来源：http://fbx.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bgy.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xxn.havefunace.top

[Q76] 按天统计
来源：http://lly.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ent.havefunace.top

[Q77] 时间加减
来源：http://twq.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rvc.316326.xyz

[Q78] 当前时间
来源：http://dgm.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gjm.yuxming.cn

[Q79] 字符串拼接
来源：http://tbv.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://inz.316326.xyz

[Q80] 字符串截取
来源：http://ymq.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hqy.aibaodan.cn

[Q81] 字符串替换
来源：http://dia.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://obx.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://gqi.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aog.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://yxw.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ood.52xcode.cn

[Q84] 去除首尾空格
来源：http://ymg.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://cjq.zhengqikj.top

[Q85] 数值取整
来源：http://azc.kuanghao11.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ilu.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://jqu.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://msq.52xcode.cn

[Q87] JSON 字段做条件
来源：http://mru.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cuo.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://bdt.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yvo.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://obs.fehbvm.com

[Q89] 判断表是否存在
来源：http://zcg.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kte.shuidangran.top

[Q90] 生成序号列
来源：http://tpt.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oxe.aizwys.cn

================================================================================
来源：http://att.hysaishi.cn

R. Bash 专题
来源：http://scv.svipenyu.cn

================================================================================
来源：http://fvg.hcnkem.com

[R01] shebang 与严格模式
来源：http://zfp.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://rug.pycfn.com

set -euo pipefail
来源：http://czz.vehdjk.com

[R02] 变量赋值与使用
来源：http://fex.yj202588.top

name="Tom"; echo "$name"
来源：http://aan.jinqigufen.top

[R03] 只读变量
来源：http://pld.pengpengdd.cyou

readonly PI=3.14
来源：http://bwv.shuidangran.top

[R04] 位置参数
来源：http://hii.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lzo.cqqwz.cn

[R05] 参数默认值
来源：http://zog.ivvv.top

name="${1:-default}"
来源：http://rch.aizwys.cn

[R06] 判断命令是否存在
来源：http://ftb.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xhk.gzhubu.top

[R07] if 判断文件
来源：http://abw.chenjidiqi.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ced.zhengqikj.top

[R08] 数值比较
来源：http://fgp.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sct.svipenyu.cn

[R09] 字符串比较
来源：http://jny.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dua.mhx1999.top

[R10] 正则匹配
来源：http://bxy.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tvm.chenlongwang.top

[R11] case 多分支
来源：http://dos.vqdsnc.cn

case "$1" in
来源：http://bha.zhoulong.xyz

start) echo "启动" ;;
来源：http://hdu.hesvh.cn

stop)  echo "停止" ;;
来源：http://xru.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://pzt.sxryk.cn

esac
来源：http://xdp.chenjidiqi.icu

[R12] for 遍历文件
来源：http://yxf.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://myy.hammf.cn

[R13] for 计数循环
来源：http://rcw.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://kxg.zhixingplan.top

[R14] C 风格 for
来源：http://qcu.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oey.gogol.net.cn

[R15] while 逐行读文件
来源：http://fno.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://htq.xziqi.cn

[R16] until 等待条件
来源：http://bna.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uuw.sysykeji.top

[R17] 数组定义与取值
来源：http://epo.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://uuj.fanxiaobao.xyz

[R18] 遍历数组
来源：http://rqq.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mhz.ywan-chungtsiang.top

[R19] 数组长度
来源：http://yhy.tianlin.xyz

echo "${#arr[@]}"
来源：http://qbs.bjfxy.top

[R20] 关联数组（字典）
来源：http://swh.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dck.mhx1999.top

[R21] 字符串长度
来源：http://srp.zdqjudy.top

echo "${#s}"
来源：http://uns.zdqjudy.top

[R22] 截取子串
来源：http://awx.dashuyun.cn

echo "${s:0:5}"
来源：http://itn.zhengqikj.top

[R23] 字符串替换
来源：http://tqj.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mfa.hnqzz.top

[R24] 大小写转换
来源：http://udi.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://xue.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://uyp.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bee.fengsongda.top

[R26] 命令替换
来源：http://srk.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://ffp.tian-w.cn

[R27] 算术展开
来源：http://ypr.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://cnh.sjlbkw.cn

[R28] 浮点运算
来源：http://wbb.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://nmv.andypj.xyz

[R29] 定义函数
来源：http://sup.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ikv.sxryk.cn

[R30] 函数返回状态码
来源：http://sla.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://ysg.andypj.xyz

[R31] 局部变量
来源：http://vyc.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://gpk.yuanzhike.top

[R32] 参数个数校验
来源：http://oha.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ywo.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://iip.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eav.xuetiantiany.cn

[R34] 退出时清理
来源：http://mro.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://fzh.quarkkingdee.top

[R35] 后台执行并等待
来源：http://knd.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xgo.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://qfu.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://grk.mhx1999.top

[R37] 把输出赋给变量
来源：http://srm.yj20258888.top

files=$(ls -1)
来源：http://hnv.dashuyun.cn

[R38] 管道串联
来源：http://fwl.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://rys.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://obc.xylfe.cn

cmd > out.log 2>&1
来源：http://pma.yangfankeji.com

[R40] 追加写日志
来源：http://ymv.xuanzx.com

echo "log" >> out.log
来源：http://hra.yongpay.top

[R41] 丢弃输出
来源：http://isd.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://tyn.ehwqpu.com

[R42] 输入重定向
来源：http://eva.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://jwn.jianghu66.top

[R43] 按名字查找文件
来源：http://syz.yuanzhike.top

find . -name "*.log" -type f
来源：http://jlc.jinqigfzy.top

[R44] 按修改时间查找
来源：http://bfp.cheryme.top

find . -mtime -7 -type f
来源：http://tfe.jinyuanbaomall.cn

[R45] 批量删除
来源：http://brv.316326.xyz

find . -name "*.tmp" -delete
来源：http://zyc.hammf.cn

[R46] 递归替换文件内容
来源：http://ppy.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ldp.hysaishi.cn

[R47] sed 单行替换
来源：http://kjo.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://giy.zdqjudy.top

[R48] awk 取指定列
来源：http://mdj.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://cbz.hnqzz.top

[R49] awk 带条件
来源：http://rbq.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aky.svipenyu.cn

[R50] awk 求和
来源：http://jdu.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ias.0kj1m.cn

[R51] 排序去重取前几
来源：http://jnn.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aqm.kuanghao11.cn

[R52] 统计行数
来源：http://oqx.yueranfly.top

wc -l a.txt
来源：http://lai.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://avx.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rtx.fehbvm.com

[R54] 比较两个文件
来源：http://taq.yfazqb.com

diff a.txt b.txt
来源：http://ejx.nanxuanxn.top

[R55] 压缩与解压
来源：http://xjn.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://apj.xylfe.cn

[R56] 远程拷贝
来源：http://ysq.pengpengdd.cyou

scp file user@host:/path/
来源：http://inf.gotoacloud.top

[R57] 远程执行命令
来源：http://aol.jinqigfzy.top

ssh user@host 'uptime'
来源：http://caa.jinqigfzy.top

[R58] 下载文件
来源：http://ezk.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hxg.yvedp.cn

[R59] 发 POST JSON
来源：http://ayh.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ttt.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://woe.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xgf.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://iwa.yuanzhike.top

df -h;  du -sh *
来源：http://tkg.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://pjj.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://bwb.wangshuangyany.cn

[R63] 内存与进程
来源：http://vzz.yj20258.top

free -h;  ps aux | grep nginx
来源：http://ynv.fehbvm.com

[R64] 结束进程
来源：http://okm.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://zje.zhongyouzk.top

[R65] 查看端口占用
来源：http://mqa.c1oappe.top


<!-- 参考信息 -->