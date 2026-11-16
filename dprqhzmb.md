代发 wailian999

[Q36] 左连接
来源：http://uus.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://okq.nanxinkj.top

[Q37] 右连接
来源：http://muj.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vos.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ebh.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hta.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://qiv.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fiv.aibaodan.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://efw.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://srh.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xpu.hnqzz.top

[Q41] 多表连接
来源：http://iqf.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hzr.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://rjd.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://pxn.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://vpp.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://whu.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hkm.jinqigfzy.top

[Q43] 标量子查询
来源：http://zaw.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rzu.svipenyu.cn

[Q44] IN 子查询
来源：http://qvm.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dss.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://tyj.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ocf.guannengcc.top

[Q46] NOT EXISTS 判断不存在
来源：http://hvy.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nie.zhijiandao.cn

[Q47] 与平均值比较
来源：http://vso.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wgk.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://utw.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lfa.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://ifp.yuanzhike.top

[Q49] 更新单行
来源：http://yvd.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ore.cdnleiting.top

[Q50] 批量更新
来源：http://zta.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://von.jqgfzy.top

[Q51] 用子查询更新
来源：http://wks.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lme.shuidangran.top

[Q52] 删除指定行
来源：http://tjb.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://uzm.bbcook.cn

[Q53] 按条件删除
来源：http://pyn.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ear.hnqzz.top

[Q54] 清空表
来源：http://cos.yj20258.top

TRUNCATE TABLE logs;
来源：http://sbv.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://pwn.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ryv.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://srz.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kvw.zdqjudy.top

[Q57] 行号
来源：http://ppz.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xgz.hcnkem.com

[Q58] 累计求和
来源：http://foq.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dkh.hcnkem.com

[Q59] 分组内累计
来源：http://gtc.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://otl.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://mei.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://snk.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://koi.yfazqb.com

[Q61] 移动平均
来源：http://fba.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tfe.sufxvd.cn

[Q62] 分组占比
来源：http://ixu.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fqp.zhiwuduotai.top

[Q63] 开启事务
来源：http://wzc.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cpc.ivvv.top

[Q64] 提交事务
来源：http://pmx.hnqzz.top

COMMIT;
来源：http://bba.yfazqb.com

[Q65] 回滚事务
来源：http://tux.quarkkingdee.top

ROLLBACK;
来源：http://swl.pengpengdd.cyou

[Q66] 行锁查询
来源：http://ivk.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ajf.chenlongwang.top

[Q67] 设置隔离级别
来源：http://cts.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hwj.wangshuangyany.cn

[Q68] 保存点
来源：http://ohb.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://dxh.zdqjudy.top

ROLLBACK TO sp1;
来源：http://mqi.zhoulong.xyz

[Q69] 查看执行计划
来源：http://qnn.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xhu.ivvv.top

[Q70] 更新统计信息
来源：http://exs.xinyue.icu

ANALYZE TABLE users;
来源：http://fwp.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://tkr.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ytr.yvedp.cn

[Q72] 查看索引
来源：http://cew.vehdjk.com

SHOW INDEX FROM users;
来源：http://ova.fehbvm.com

[Q73] 查看表状态
来源：http://yaz.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ziu.shzxlz.cn

[Q74] 强制使用索引
来源：http://lzt.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eut.bbcook.cn

[Q75] 日期格式化
来源：http://yzx.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cqw.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lmc.pycfn.com

[Q76] 按天统计
来源：http://mvj.jyoumei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rsp.xinyue.icu

[Q77] 时间加减
来源：http://vvo.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://los.hnqzz.top

[Q78] 当前时间
来源：http://bzh.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dwo.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://etw.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://equ.jianghu66.top

[Q80] 字符串截取
来源：http://bfq.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://omj.jinqigufen.top

[Q81] 字符串替换
来源：http://cbj.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uah.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://sue.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://avl.hongshengwenyu.top

[Q83] 大小写转换
来源：http://yvm.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ban.zdqjudy.top

[Q84] 去除首尾空格
来源：http://ewh.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://aan.jlsjyb.cn

[Q85] 数值取整
来源：http://vvi.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rrh.ivvv.top

[Q86] 读取 JSON 字段
来源：http://qbb.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fll.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://eek.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrh.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://dnd.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qsy.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dwg.daxiang520.top

[Q89] 判断表是否存在
来源：http://xvc.sxryk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ieg.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://nes.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jjx.tianlin.xyz

================================================================================
来源：http://iiu.redwolf501.top

R. Bash 专题
来源：http://qaq.yangfankeji.com

================================================================================
来源：http://les.jianghu66.top

[R01] shebang 与严格模式
来源：http://day.fktsv.cn

#!/usr/bin/env bash
来源：http://ysw.jyoumei.cn

set -euo pipefail
来源：http://ofr.tian-w.cn

[R02] 变量赋值与使用
来源：http://tyr.jinqigufen.top

name="Tom"; echo "$name"
来源：http://wdm.zhixingplan.top

[R03] 只读变量
来源：http://gbk.ehwqpu.com

readonly PI=3.14
来源：http://zxm.guowangkeji.top

[R04] 位置参数
来源：http://dfm.guowangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xyl.xziqi.cn

[R05] 参数默认值
来源：http://cey.ppjwa.cn

name="${1:-default}"
来源：http://dpr.sysykeji.top

[R06] 判断命令是否存在
来源：http://wnh.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ncp.yj202588.top

[R07] if 判断文件
来源：http://wxa.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqc.hywenlv.cn

[R08] 数值比较
来源：http://gkh.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://wem.hnqzz.top

[R09] 字符串比较
来源：http://biq.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cwb.gotoacloud.top

[R10] 正则匹配
来源：http://pwq.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xog.jinqigufen.top

[R11] case 多分支
来源：http://bpw.tanke756.top

case "$1" in
来源：http://qjd.jiagoushi.top

start) echo "启动" ;;
来源：http://btn.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://btp.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://zxg.shanyushiyangtech.top

esac
来源：http://fpj.yonumen.top

[R12] for 遍历文件
来源：http://hwe.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://cio.xinyue.icu

[R13] for 计数循环
来源：http://idg.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://fpp.zhengqikj.top

[R14] C 风格 for
来源：http://mlf.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sse.haohaochexian.top

[R15] while 逐行读文件
来源：http://gsn.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cwn.yonumen.top

[R16] until 等待条件
来源：http://wuj.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zbn.yj20258.top

[R17] 数组定义与取值
来源：http://mxa.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://jqx.gaohongyu789.top

[R18] 遍历数组
来源：http://hos.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mzp.feifeiyinyue.top

[R19] 数组长度
来源：http://lpu.pycfn.com

echo "${#arr[@]}"
来源：http://vfa.cashguo.top

[R20] 关联数组（字典）
来源：http://mzg.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zjp.guannengcc.top

[R21] 字符串长度
来源：http://ydz.redwolf501.top

echo "${#s}"
来源：http://mpj.xuanzx.com

[R22] 截取子串
来源：http://dkx.fktsv.cn

echo "${s:0:5}"
来源：http://zwu.cdnleiting.top

[R23] 字符串替换
来源：http://ynz.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yjz.52xcode.cn

[R24] 大小写转换
来源：http://xor.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ilp.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://hax.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zgi.316326.xyz

[R26] 命令替换
来源：http://wpb.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://mte.sjlbkw.cn

[R27] 算术展开
来源：http://jet.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://cvt.zhijiandao.cn

[R28] 浮点运算
来源：http://bmz.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://xti.yj20258.top

[R29] 定义函数
来源：http://ugv.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://myz.aibaodan.cn

[R30] 函数返回状态码
来源：http://uas.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://mxn.cucudq.cn

[R31] 局部变量
来源：http://rke.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://vxh.wangdashe.top

[R32] 参数个数校验
来源：http://dri.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://khw.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://ios.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dpy.smart0.xyz

[R34] 退出时清理
来源：http://llz.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://goo.guannengcc.top

[R35] 后台执行并等待
来源：http://oti.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ljd.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://zfc.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://odj.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://xft.zhijiandao.cn

files=$(ls -1)
来源：http://muh.mhx1999.top

[R38] 管道串联
来源：http://mxk.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://nnp.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://lof.jlsjyb.cn

cmd > out.log 2>&1
来源：http://qhd.cheryme.top

[R40] 追加写日志
来源：http://ptw.vehdjk.com

echo "log" >> out.log
来源：http://rlw.redwolf501.top

[R41] 丢弃输出
来源：http://tfu.sweek.top

cmd >/dev/null 2>&1
来源：http://tii.316326.xyz

[R42] 输入重定向
来源：http://eqb.gotoacloud.top

wc -l < a.txt
来源：http://yru.yonumen.top

[R43] 按名字查找文件
来源：http://unj.yj202588.top

find . -name "*.log" -type f
来源：http://rsv.ydjk.org.cn

[R44] 按修改时间查找
来源：http://irt.meibo888.top

find . -mtime -7 -type f
来源：http://gpr.hywenlv.cn

[R45] 批量删除
来源：http://hsa.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://fgr.yvedp.cn

[R46] 递归替换文件内容
来源：http://ntb.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nel.gotoacloud.top

[R47] sed 单行替换
来源：http://dpx.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qlf.0kj1m.cn

[R48] awk 取指定列
来源：http://nif.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://nyu.vqdsnc.cn

[R49] awk 带条件
来源：http://lqn.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ppj.pycfn.com

[R50] awk 求和
来源：http://bmo.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jma.hcnkem.com

[R51] 排序去重取前几
来源：http://dxs.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lbp.zhoulong.xyz

[R52] 统计行数
来源：http://nru.jinyuanbaomall.cn

wc -l a.txt
来源：http://zqr.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://dkp.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hmr.zycfv.cn

[R54] 比较两个文件
来源：http://tab.haohaochexian.top

diff a.txt b.txt
来源：http://ged.jqgfzy.top

[R55] 压缩与解压
来源：http://fgl.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zqv.yuanzhike.top

[R56] 远程拷贝
来源：http://cep.shanyushiyangtech.top

scp file user@host:/path/
来源：http://ghk.smart0.xyz

[R57] 远程执行命令
来源：http://gen.gotoacloud.top

ssh user@host 'uptime'
来源：http://iyo.hfpthk.cn

[R58] 下载文件
来源：http://ruw.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vwx.pycfn.com

[R59] 发 POST JSON
来源：http://zns.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://biy.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://hes.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zgh.yj202588.top

[R61] 磁盘占用
来源：http://oop.bbcook.cn

df -h;  du -sh *
来源：http://uih.epnwcf.com

[R62] 找最占空间的文件
来源：http://xes.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://sgd.yangfankeji.com

[R63] 内存与进程
来源：http://zcf.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://nfd.yj20258888.top

[R64] 结束进程
来源：http://vor.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://kys.hesvh.cn

[R65] 查看端口占用
来源：http://ffs.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjb.fanxiaobao.xyz

[R66] 定时任务
来源：http://gkl.tianlin.xyz

crontab -e;  crontab -l
来源：http://ckp.fehbvm.com

[R67] 生成随机十六进制串
来源：http://oqu.yj20258888.top

openssl rand -hex 16
来源：http://jwq.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://bom.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://omw.bbcook.cn

[R69] 生成随机密码
来源：http://umu.cashguo.top

head -c 16 /dev/urandom | base64
来源：http://ukr.nanxinkj.top

[R70] 时间戳与互转
来源：http://srl.sweek.top

date +%s;  date -d @1700000000
来源：http://frw.dianchejie.cn

[R71] 日期格式化
来源：http://yma.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://abw.sufxvd.cn

[R72] 等待端口就绪
来源：http://sdb.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uas.yueranfly.top

[R73] 分割大日志
来源：http://czi.xinyue.icu

split -l 1000 big.log part_
来源：http://qcl.fehbvm.com

[R74] 批量重命名
来源：http://zjt.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vlj.snrcjt.cn

[R75] 导出环境变量
来源：http://puc.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://hxa.yonumen.top

[R76] 使用临时文件
来源：http://ttj.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gem.jyoumei.cn

[R77] 读取用户输入
来源：http://mvp.ydzc1.top

read -rp "请输入: " ans
来源：http://tau.ivvv.top

[R78] 交互式菜单
来源：http://axn.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://szp.tian-w.cn

[R79] 解析命令行选项
来源：http://nqn.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uua.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://oso.jqgfzy.top

time ./run.sh
来源：http://tic.jinqigfzy.top

================================================================================
来源：http://akm.yongpay.top

S. C / C++ 专题
来源：http://ozb.316326.xyz

================================================================================
来源：http://pyo.zhixingplan.top

[S01] C：Hello World
来源：http://fzd.zhixingplan.top

#include <stdio.h>
来源：http://pwb.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iqg.fzhhl.top

[S02] C：变量与格式化输出
来源：http://vxm.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://igy.jiagoushi.top

[S03] C：读入整数
来源：http://yiu.meibo888.top

int x; scanf("%d", &x);
来源：http://ijh.316326.xyz

[S04] C：字符串复制
来源：http://sae.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ldu.xuanzx.com

[S05] C：字符串长度
来源：http://wjj.jinqigufen.top


<!-- 参考信息 -->