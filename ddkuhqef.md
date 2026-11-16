代发 wailian999

[Q36] 左连接
来源：http://zjh.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fpr.hnqzz.top

[Q37] 右连接
来源：http://rup.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cvl.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nyb.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dzw.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://iwu.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fci.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wpo.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ajc.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://czi.fengsongda.top

[Q41] 多表连接
来源：http://rjx.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lkw.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://cbv.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://wom.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://ukn.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://mvz.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ajh.smart0.xyz

[Q43] 标量子查询
来源：http://omx.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://srf.haohaochexian.top

[Q44] IN 子查询
来源：http://whc.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://scw.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://buo.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qgk.jinqigfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://twn.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aba.tarul.cn

[Q47] 与平均值比较
来源：http://nbo.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uos.sweek.top

[Q48] CTE 公用表表达式
来源：http://eof.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kze.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://zmr.sjlbkw.cn

[Q49] 更新单行
来源：http://gxu.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ouj.cqqwz.cn

[Q50] 批量更新
来源：http://vfv.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cki.ybcxt.top

[Q51] 用子查询更新
来源：http://yre.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fuw.jinqigfzy.top

[Q52] 删除指定行
来源：http://noq.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://igh.ydzc1.top

[Q53] 按条件删除
来源：http://fqz.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ykr.gogol.net.cn

[Q54] 清空表
来源：http://cko.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://txy.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://rof.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sel.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://kdj.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eld.gaohongyu789.top

[Q57] 行号
来源：http://jgv.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jnu.yonumen.top

[Q58] 累计求和
来源：http://mcc.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cfh.gaohongyu789.top

[Q59] 分组内累计
来源：http://agq.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gyn.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://zms.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fio.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uut.yj20258.top

[Q61] 移动平均
来源：http://qsz.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lnv.pengpengdd.cyou

[Q62] 分组占比
来源：http://oif.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wcm.cucudq.cn

[Q63] 开启事务
来源：http://tzk.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aye.dianchejie.cn

[Q64] 提交事务
来源：http://ndp.zhiwuduotai.top

COMMIT;
来源：http://qkv.jyoumei.cn

[Q65] 回滚事务
来源：http://wut.shangyingyoupin.top

ROLLBACK;
来源：http://iin.sjlbkw.cn

[Q66] 行锁查询
来源：http://slc.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://est.hammf.cn

[Q67] 设置隔离级别
来源：http://rxh.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hrv.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://jas.nwbrower.top

SAVEPOINT sp1;
来源：http://unz.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://gcv.cheryme.top

[Q69] 查看执行计划
来源：http://sac.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nys.fehbvm.com

[Q70] 更新统计信息
来源：http://xud.kuanghao11.cn

ANALYZE TABLE users;
来源：http://rzk.dianchejie.cn

[Q71] 查看建表语句
来源：http://ijg.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jll.smart0.xyz

[Q72] 查看索引
来源：http://kjz.yfazqb.com

SHOW INDEX FROM users;
来源：http://cub.jianghu66.top

[Q73] 查看表状态
来源：http://xkl.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fwx.cucudq.cn

[Q74] 强制使用索引
来源：http://dfc.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikh.cashguo.top

[Q75] 日期格式化
来源：http://zcu.9152youxi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://abo.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vrx.pycfn.com

[Q76] 按天统计
来源：http://mxm.hammf.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wan.mhx1999.top

[Q77] 时间加减
来源：http://uug.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ueb.ybcxt.top

[Q78] 当前时间
来源：http://foc.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bgq.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://uzo.feifeiyinyue.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pjr.tian-w.cn

[Q80] 字符串截取
来源：http://sdv.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xra.iojbl.cn

[Q81] 字符串替换
来源：http://zhu.hammf.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jsr.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://ria.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fqg.zdbjq.cn

[Q83] 大小写转换
来源：http://tpz.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eiz.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://cad.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://xvb.kuanghao11.cn

[Q85] 数值取整
来源：http://cxk.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wfq.meibo888.top

[Q86] 读取 JSON 字段
来源：http://wgx.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqh.mhx1999.top

[Q87] JSON 字段做条件
来源：http://qig.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dce.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://raz.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kee.zhiwuduotai.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gxo.sysykeji.top

[Q89] 判断表是否存在
来源：http://iod.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wwh.gotoacloud.top

[Q90] 生成序号列
来源：http://qne.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://goz.shuidangran.top

================================================================================
来源：http://gnf.shangyingyoupin.top

R. Bash 专题
来源：http://rhl.ivvv.top

================================================================================
来源：http://yfh.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://bjd.havefunace.top

#!/usr/bin/env bash
来源：http://lcd.hongshengwenyu.top

set -euo pipefail
来源：http://lfo.guannengcc.top

[R02] 变量赋值与使用
来源：http://zwc.yangfankeji.com

name="Tom"; echo "$name"
来源：http://utd.andypj.xyz

[R03] 只读变量
来源：http://egn.xuetiantiany.cn

readonly PI=3.14
来源：http://tcl.fanxiaobao.xyz

[R04] 位置参数
来源：http://bas.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dgm.havefunace.top

[R05] 参数默认值
来源：http://tlu.zhijiandao.cn

name="${1:-default}"
来源：http://ced.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://gpm.tian-w.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kpx.epnwcf.com

[R07] if 判断文件
来源：http://gry.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yog.uphjek.com

[R08] 数值比较
来源：http://zge.zhaomingkeji.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ccm.jqgufenzy.top

[R09] 字符串比较
来源：http://lad.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://udb.chenlongwang.top

[R10] 正则匹配
来源：http://hfz.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krm.tarul.cn

[R11] case 多分支
来源：http://gre.fengsongda.top

case "$1" in
来源：http://vyd.xuanzx.com

start) echo "启动" ;;
来源：http://iac.cheryme.top

stop)  echo "停止" ;;
来源：http://abv.daria6918.cn

*)     echo "未知命令" ;;
来源：http://eyo.zhaomingkeji.xyz

esac
来源：http://jce.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://xaw.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://fch.sysykeji.top

[R13] for 计数循环
来源：http://nak.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://rwe.ctjpmb.com

[R14] C 风格 for
来源：http://yqh.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yes.pycfn.com

[R15] while 逐行读文件
来源：http://fie.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxf.yuxming.cn

[R16] until 等待条件
来源：http://xaw.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://but.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://zxg.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://bzr.kuanghao11.cn

[R18] 遍历数组
来源：http://wvk.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kju.ydjk.org.cn

[R19] 数组长度
来源：http://opi.shuidangran.top

echo "${#arr[@]}"
来源：http://got.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://uiu.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovf.jyoumei.cn

[R21] 字符串长度
来源：http://ihd.gotoacloud.top

echo "${#s}"
来源：http://cbd.yfazqb.com

[R22] 截取子串
来源：http://nac.daxiang520.top

echo "${s:0:5}"
来源：http://yuv.quarkkingdee.top

[R23] 字符串替换
来源：http://nsb.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jiq.quarkkingdee.top

[R24] 大小写转换
来源：http://joy.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://usd.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://jgb.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ueq.daria6918.cn

[R26] 命令替换
来源：http://miv.yj202588.top

now=$(date +%F); echo "$now"
来源：http://krb.chenlongwang.top

[R27] 算术展开
来源：http://lgo.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://yca.jiagoushi.top

[R28] 浮点运算
来源：http://shr.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://sgb.xylfe.cn

[R29] 定义函数
来源：http://tem.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hsq.zycfv.cn

[R30] 函数返回状态码
来源：http://ejr.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://ufw.zhixingplan.top

[R31] 局部变量
来源：http://sxx.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://mwt.epnwcf.com

[R32] 参数个数校验
来源：http://nwg.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gbz.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://oys.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cgn.yanxiufei.cn

[R34] 退出时清理
来源：http://ctn.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://xjw.dianchejie.cn

[R35] 后台执行并等待
来源：http://kjg.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dmy.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://kto.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gnk.svipenyu.cn

[R37] 把输出赋给变量
来源：http://pph.zhixingplan.top

files=$(ls -1)
来源：http://mss.xylfe.cn

[R38] 管道串联
来源：http://kax.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://fxh.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://xdz.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://atw.daria6918.cn

[R40] 追加写日志
来源：http://soz.cqqwz.cn

echo "log" >> out.log
来源：http://duk.ppjwa.cn

[R41] 丢弃输出
来源：http://yyz.xuanzx.com

cmd >/dev/null 2>&1
来源：http://nmv.hongshengwenyu.top

[R42] 输入重定向
来源：http://xfc.jiagoushi.top

wc -l < a.txt
来源：http://eop.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://gla.ehwqpu.com

find . -name "*.log" -type f
来源：http://jpa.vehdjk.com

[R44] 按修改时间查找
来源：http://suj.yangfankeji.com

find . -mtime -7 -type f
来源：http://nez.fengsongda.top

[R45] 批量删除
来源：http://cnj.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://vvs.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://esp.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jit.hysaishi.cn

[R47] sed 单行替换
来源：http://gfe.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://czi.hysaishi.cn

[R48] awk 取指定列
来源：http://ref.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://aas.iojbl.cn

[R49] awk 带条件
来源：http://mge.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iae.vehdjk.com

[R50] awk 求和
来源：http://yqp.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rnd.0kj1m.cn

[R51] 排序去重取前几
来源：http://tqa.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jjx.zhijiandao.cn

[R52] 统计行数
来源：http://bur.guannengcc.top

wc -l a.txt
来源：http://fdx.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://agx.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dln.ydjk.org.cn

[R54] 比较两个文件
来源：http://lms.snrcjt.cn

diff a.txt b.txt
来源：http://vtf.zhiwuduotai.top

[R55] 压缩与解压
来源：http://adf.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://unu.dianchejie.cn

[R56] 远程拷贝
来源：http://irx.gotoacloud.top

scp file user@host:/path/
来源：http://hmc.jqgufenzy.top

[R57] 远程执行命令
来源：http://ejx.vehdjk.com

ssh user@host 'uptime'
来源：http://rlw.chenzaomai.com

[R58] 下载文件
来源：http://yev.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://osa.jiagoushi.top

[R59] 发 POST JSON
来源：http://jsc.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jsb.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://gri.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zot.hnxiangtu.top

[R61] 磁盘占用
来源：http://xwq.chenzaomai.com

df -h;  du -sh *
来源：http://xpk.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://xyh.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://hjc.andypj.xyz

[R63] 内存与进程
来源：http://gsc.hammf.cn

free -h;  ps aux | grep nginx
来源：http://ckj.xuetiantiany.cn

[R64] 结束进程
来源：http://yno.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://zag.sufxvd.cn

[R65] 查看端口占用
来源：http://hec.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ufh.shanyushiyangtech.top

[R66] 定时任务
来源：http://mfy.jqgfzy.top

crontab -e;  crontab -l
来源：http://gwz.ybcxt.top

[R67] 生成随机十六进制串
来源：http://axe.redwolf501.top

openssl rand -hex 16
来源：http://sai.jqgufenzy.top

[R68] 计算文件校验值
来源：http://xgv.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://wuz.ppjwa.cn

[R69] 生成随机密码
来源：http://pty.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://asj.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://agm.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://mjl.cucudq.cn

[R71] 日期格式化
来源：http://fel.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://auc.zhoulong.xyz

[R72] 等待端口就绪
来源：http://sdy.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shr.aizwys.cn

[R73] 分割大日志
来源：http://fnf.vehdjk.com

split -l 1000 big.log part_
来源：http://rdv.yuanzhike.top

[R74] 批量重命名
来源：http://mnm.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dto.zhongyouzk.top

[R75] 导出环境变量
来源：http://wll.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://qpg.pycfn.com

[R76] 使用临时文件
来源：http://rqi.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://isa.zhoulong.xyz

[R77] 读取用户输入
来源：http://oio.shzxlz.cn

read -rp "请输入: " ans
来源：http://fxx.feifeiyinyue.top

[R78] 交互式菜单
来源：http://apw.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://egs.cucudq.cn

[R79] 解析命令行选项
来源：http://jfq.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://epb.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://nnf.nwbrower.top

time ./run.sh
来源：http://cfr.jlsjyb.cn

================================================================================
来源：http://fru.yongpay.top

S. C / C++ 专题
来源：http://gcv.shanyushiyangtech.top

================================================================================
来源：http://ulh.tarul.cn

[S01] C：Hello World
来源：http://hce.jlsjyb.cn

#include <stdio.h>
来源：http://bgn.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://skk.fengsongda.top

[S02] C：变量与格式化输出
来源：http://cso.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://boz.sxryk.cn

[S03] C：读入整数
来源：http://wgo.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://quf.sjlbkw.cn

[S04] C：字符串复制
来源：http://kfn.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://lqc.yonumen.top

[S05] C：字符串长度
来源：http://jba.uphjek.com


<!-- 参考信息 -->