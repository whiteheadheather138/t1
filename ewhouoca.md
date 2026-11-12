代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tuh.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://tmy.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eyr.jyoumei.cn

[Q19] 范围查询
来源：http://lea.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gwg.ppjwa.cn

[Q20] IN 列表
来源：http://trb.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dir.0kj1m.cn

[Q21] 空值判断
来源：http://vcz.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ndz.ctjpmb.com

[Q22] 排序
来源：http://kmu.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://joy.jinqigufen.top

[Q23] 分页
来源：http://qye.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bys.haohaochexian.top

[Q24] 去重
来源：http://jqb.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://zut.havefunace.top

[Q25] 只取前 N 条
来源：http://bag.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ykc.ehwqpu.com

[Q26] 计数
来源：http://igi.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://zdy.xuanzx.com

[Q27] 条件计数
来源：http://knu.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vvl.jyoumei.cn

[Q28] 求和与平均
来源：http://wzl.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cms.0kj1m.cn

[Q29] 最大最小值
来源：http://xdb.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://amp.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://mvm.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xbq.yonumen.top

[Q31] 分组后过滤
来源：http://wxw.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ozw.shuidangran.top

[Q32] 分组拼接字符串
来源：http://xyf.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mtk.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://osx.sysykeji.top

[Q33] 多列分组
来源：http://isq.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wvn.vehdjk.com

[Q34] 每组取第一条
来源：http://uag.xinyue.icu

SELECT * FROM (
来源：http://kgp.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pjz.sxryk.cn

) t WHERE rn = 1;
来源：http://dcs.jinqigufen.top

[Q35] 内连接
来源：http://rhy.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pad.ehwqpu.com

[Q36] 左连接
来源：http://vyi.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nql.ywan-chungtsiang.top

[Q37] 右连接
来源：http://xal.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://usz.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oqf.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sud.nanxinkj.top

[Q39] 自连接（查上下级）
来源：http://yip.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tqn.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hmh.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://hcm.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rll.haohaochexian.top

[Q41] 多表连接
来源：http://wmi.ydjk.org.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://orf.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://jga.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://bog.havefunace.top

[Q42] 连接条件附加过滤
来源：http://dmf.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://hck.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qcz.cdnleiting.top

[Q43] 标量子查询
来源：http://xec.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dyv.jianghu66.top

[Q44] IN 子查询
来源：http://fsf.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xau.yj20258.top

[Q45] EXISTS 判断存在
来源：http://ocx.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bna.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://bbw.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uto.yuanzhike.top

[Q47] 与平均值比较
来源：http://qzv.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ygu.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://yjx.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kms.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://yzd.shuidangran.top

[Q49] 更新单行
来源：http://njd.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wfw.zhongyouzk.top

[Q50] 批量更新
来源：http://aqg.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://duw.kuanghao11.cn

[Q51] 用子查询更新
来源：http://xms.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vtw.gotoacloud.top

[Q52] 删除指定行
来源：http://rby.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://vmq.tianlin.xyz

[Q53] 按条件删除
来源：http://mps.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mgp.chenzaomai.com

[Q54] 清空表
来源：http://igi.c1oappe.top

TRUNCATE TABLE logs;
来源：http://gpw.yuxming.cn

[Q55] 排名（并列占位）
来源：http://gzo.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vlm.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://jzw.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rwa.jiagoushi.top

[Q57] 行号
来源：http://jnv.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lnm.zycfv.cn

[Q58] 累计求和
来源：http://kfl.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rwk.quarkkingdee.top

[Q59] 分组内累计
来源：http://pav.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ekr.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://cyi.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pos.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vub.iojbl.cn

[Q61] 移动平均
来源：http://vxe.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gnq.gaohongyu789.top

[Q62] 分组占比
来源：http://sdg.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rus.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://sbm.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ptw.cucudq.cn

[Q64] 提交事务
来源：http://ygo.zdbjq.cn

COMMIT;
来源：http://lwp.zhijiandao.cn

[Q65] 回滚事务
来源：http://rai.zhijiandao.cn

ROLLBACK;
来源：http://vpd.tanke756.top

[Q66] 行锁查询
来源：http://wjc.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eml.xinyue.icu

[Q67] 设置隔离级别
来源：http://mgy.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vsd.c1oappe.top

[Q68] 保存点
来源：http://oau.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://cty.iojbl.cn

ROLLBACK TO sp1;
来源：http://pnd.nanxinkj.top

[Q69] 查看执行计划
来源：http://rsr.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qok.jqgfzy.top

[Q70] 更新统计信息
来源：http://mun.haohaochexian.top

ANALYZE TABLE users;
来源：http://yjt.zhixingplan.top

[Q71] 查看建表语句
来源：http://shn.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://onr.xziqi.cn

[Q72] 查看索引
来源：http://kay.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://ulx.cashguo.top

[Q73] 查看表状态
来源：http://xgr.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dlo.jyoumei.cn

[Q74] 强制使用索引
来源：http://hzu.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://arn.sysykeji.top

[Q75] 日期格式化
来源：http://xfx.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ryc.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fwz.tianlin.xyz

[Q76] 按天统计
来源：http://ndz.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xld.jinghuilouyu.cn

[Q77] 时间加减
来源：http://ilo.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lwe.9152youxi.cn

[Q78] 当前时间
来源：http://dll.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uhf.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://hlw.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yhq.gotoacloud.top

[Q80] 字符串截取
来源：http://kux.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ury.daria6918.cn

[Q81] 字符串替换
来源：http://btp.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wml.yj20258.top

[Q82] 字符长度与字节长度
来源：http://vsx.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vih.sjlbkw.cn

[Q83] 大小写转换
来源：http://zeu.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eme.yuanzhike.top

[Q84] 去除首尾空格
来源：http://ona.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://nzh.gotoacloud.top

[Q85] 数值取整
来源：http://gkn.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xfg.ivvv.top

[Q86] 读取 JSON 字段
来源：http://hiu.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hiy.sweek.top

[Q87] JSON 字段做条件
来源：http://qdi.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wka.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://tjd.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lak.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nsx.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://eva.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kbd.guannengcc.top

[Q90] 生成序号列
来源：http://zsr.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://amx.nanxuanxn.top

================================================================================
来源：http://uca.nanxuanxn.top

R. Bash 专题
来源：http://euf.xylfe.cn

================================================================================
来源：http://fsn.hysaishi.cn

[R01] shebang 与严格模式
来源：http://qxp.bjfxy.top

#!/usr/bin/env bash
来源：http://zuo.zhijiandao.cn

set -euo pipefail
来源：http://yyr.iojbl.cn

[R02] 变量赋值与使用
来源：http://hxz.yvedp.cn

name="Tom"; echo "$name"
来源：http://fpi.cheryme.top

[R03] 只读变量
来源：http://ada.zhaomingkeji.xyz

readonly PI=3.14
来源：http://ihv.nanxuanxn.top

[R04] 位置参数
来源：http://nht.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://snu.fengsongda.top

[R05] 参数默认值
来源：http://npi.feifeiyinyue.top

name="${1:-default}"
来源：http://tra.0kj1m.cn

[R06] 判断命令是否存在
来源：http://zfs.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qlc.tian-w.cn

[R07] if 判断文件
来源：http://coo.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ten.kuanghao11.cn

[R08] 数值比较
来源：http://oap.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://osc.0kj1m.cn

[R09] 字符串比较
来源：http://shq.shanyushiyangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://azy.guannengcc.top

[R10] 正则匹配
来源：http://emi.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gel.yuxming.cn

[R11] case 多分支
来源：http://fjs.shuidangran.top

case "$1" in
来源：http://csk.zdbjq.cn

start) echo "启动" ;;
来源：http://ltu.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://vdv.yongpay.top

*)     echo "未知命令" ;;
来源：http://fwo.shanyushiyangkeji.top

esac
来源：http://foy.chenzaomai.com

[R12] for 遍历文件
来源：http://bgj.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://ljz.zycfv.cn

[R13] for 计数循环
来源：http://kea.zhoulong.xyz

for i in {1..10}; do echo "$i"; done
来源：http://aei.tanke756.top

[R14] C 风格 for
来源：http://ked.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vzt.sjlbkw.cn

[R15] while 逐行读文件
来源：http://lev.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mhd.gaohongyu789.top

[R16] until 等待条件
来源：http://ynj.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://has.316326.xyz

[R17] 数组定义与取值
来源：http://cqj.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://wrr.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://guv.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dlu.jiagoushi.top

[R19] 数组长度
来源：http://kez.52xcode.cn

echo "${#arr[@]}"
来源：http://wbh.jiagoushi.top

[R20] 关联数组（字典）
来源：http://gqi.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jye.jinghuilouyu.cn

[R21] 字符串长度
来源：http://zfx.cdnleiting.top

echo "${#s}"
来源：http://ulb.yj20258.top

[R22] 截取子串
来源：http://wol.yj20258888.top

echo "${s:0:5}"
来源：http://bbf.guannengcc.top

[R23] 字符串替换
来源：http://xhn.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cgy.sysykeji.top

[R24] 大小写转换
来源：http://dxb.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cff.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://zgf.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mnr.sjlbkw.cn

[R26] 命令替换
来源：http://szv.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://siw.guowangkeji.top

[R27] 算术展开
来源：http://reg.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://ntc.dashuyun.cn

[R28] 浮点运算
来源：http://snq.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://rtz.mhx1999.top

[R29] 定义函数
来源：http://aij.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rwl.hnxiangtu.top

[R30] 函数返回状态码
来源：http://bmw.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://vhu.mhx1999.top

[R31] 局部变量
来源：http://taf.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://amq.shuidangran.top

[R32] 参数个数校验
来源：http://kit.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zza.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://pao.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbm.yj20258888.top

[R34] 退出时清理
来源：http://xvg.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://ttg.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://mxl.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hfv.tian-w.cn

[R36] 并发执行多个任务
来源：http://psf.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kse.yongpay.top

[R37] 把输出赋给变量
来源：http://gub.shanyushiyangkeji.top

files=$(ls -1)
来源：http://fhz.birdmap.top

[R38] 管道串联
来源：http://sgn.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://wbj.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://pbq.yuanzhike.top

cmd > out.log 2>&1
来源：http://wut.ydzc1.top

[R40] 追加写日志
来源：http://ape.havefunace.top

echo "log" >> out.log
来源：http://rlu.andypj.xyz

[R41] 丢弃输出
来源：http://nsm.epnwcf.com

cmd >/dev/null 2>&1
来源：http://tiv.yj20258888.top

[R42] 输入重定向
来源：http://foi.316326.xyz

wc -l < a.txt
来源：http://brx.sjlbkw.cn

[R43] 按名字查找文件
来源：http://uur.cdnleiting.top

find . -name "*.log" -type f
来源：http://uff.jianghu66.top

[R44] 按修改时间查找
来源：http://jvu.iojbl.cn

find . -mtime -7 -type f
来源：http://kiw.zhongyouzk.top

[R45] 批量删除
来源：http://odk.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://uha.316326.xyz

[R46] 递归替换文件内容
来源：http://uvc.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sil.jqgufenzy.top

[R47] sed 单行替换
来源：http://xon.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hhp.0kj1m.cn

[R48] awk 取指定列
来源：http://cvl.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://qxj.hysaishi.cn

[R49] awk 带条件
来源：http://vhm.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fui.kuanghao11.cn

[R50] awk 求和
来源：http://dha.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://nau.ydzc1.top

[R51] 排序去重取前几
来源：http://vje.316326.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://cvr.yfazqb.com

[R52] 统计行数
来源：http://kyw.shanyushiyangtech.top

wc -l a.txt
来源：http://hnr.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://ktg.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sof.yonumen.top

[R54] 比较两个文件
来源：http://nxg.fktsv.cn

diff a.txt b.txt
来源：http://xno.xuetiantiany.cn

[R55] 压缩与解压
来源：http://ccw.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fpo.hesvh.cn

[R56] 远程拷贝
来源：http://dje.pycfn.com

scp file user@host:/path/
来源：http://mcg.cdnleiting.top

[R57] 远程执行命令
来源：http://xbk.0kj1m.cn

ssh user@host 'uptime'
来源：http://nfc.hysaishi.cn

[R58] 下载文件
来源：http://mno.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://keb.yj20258888.top

[R59] 发 POST JSON
来源：http://ayz.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cek.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://kqo.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rkh.meibo888.top

[R61] 磁盘占用
来源：http://byo.52xcode.cn

df -h;  du -sh *
来源：http://sed.birdmap.top

[R62] 找最占空间的文件
来源：http://fin.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://ghg.0kj1m.cn

[R63] 内存与进程
来源：http://ftb.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://yxt.hongshengwenyu.top

[R64] 结束进程
来源：http://zga.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://trd.yfazqb.com

[R65] 查看端口占用
来源：http://cax.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://god.316326.xyz

[R66] 定时任务
来源：http://mhc.ydjk.org.cn

crontab -e;  crontab -l
来源：http://bez.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://vhq.gzhubu.top


<!-- 参考信息 -->