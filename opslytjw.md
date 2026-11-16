代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eqy.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oky.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://msh.snrcjt.cn

[Q41] 多表连接
来源：http://wrn.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ohl.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://bpw.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://sih.meibo888.top

[Q42] 连接条件附加过滤
来源：http://gyl.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://bjy.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sbf.svipenyu.cn

[Q43] 标量子查询
来源：http://bky.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kzc.smart0.xyz

[Q44] IN 子查询
来源：http://xph.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qsc.ybcxt.top

[Q45] EXISTS 判断存在
来源：http://vim.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://swa.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://sve.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tls.yfazqb.com

[Q47] 与平均值比较
来源：http://bbg.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gme.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://fpv.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mjf.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://ssr.bjfxy.top

[Q49] 更新单行
来源：http://eyj.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jmo.jyoumei.cn

[Q50] 批量更新
来源：http://veb.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oqs.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://roo.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ihn.nanxinkj.top

[Q52] 删除指定行
来源：http://gvk.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://tzv.zycfv.cn

[Q53] 按条件删除
来源：http://ddd.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qms.hnqzz.top

[Q54] 清空表
来源：http://eko.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://zkc.smart0.xyz

[Q55] 排名（并列占位）
来源：http://xdg.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aud.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://qts.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fej.sweek.top

[Q57] 行号
来源：http://vgt.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gyy.vehdjk.com

[Q58] 累计求和
来源：http://hlo.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jjp.sxryk.cn

[Q59] 分组内累计
来源：http://fnk.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gyo.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://pch.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rfz.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://djb.hesvh.cn

[Q61] 移动平均
来源：http://nqc.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hsm.xylfe.cn

[Q62] 分组占比
来源：http://gdx.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xyk.sjlbkw.cn

[Q63] 开启事务
来源：http://dft.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://erz.sxryk.cn

[Q64] 提交事务
来源：http://jzj.ydjk.org.cn

COMMIT;
来源：http://pca.aibaodan.cn

[Q65] 回滚事务
来源：http://rmn.gaohongyu789.top

ROLLBACK;
来源：http://piy.hysaishi.cn

[Q66] 行锁查询
来源：http://his.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://clm.cucudq.cn

[Q67] 设置隔离级别
来源：http://nym.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rqy.jqgufenzy.top

[Q68] 保存点
来源：http://wkf.gaohongyu789.top

SAVEPOINT sp1;
来源：http://yiz.52xcode.cn

ROLLBACK TO sp1;
来源：http://atd.hfpthk.cn

[Q69] 查看执行计划
来源：http://vqy.ctjpmb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hpy.haohaochexian.top

[Q70] 更新统计信息
来源：http://nqu.vqdsnc.cn

ANALYZE TABLE users;
来源：http://aos.aibaodan.cn

[Q71] 查看建表语句
来源：http://cjz.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uok.dashuyun.cn

[Q72] 查看索引
来源：http://bqa.iojbl.cn

SHOW INDEX FROM users;
来源：http://maw.c1oappe.top

[Q73] 查看表状态
来源：http://ebz.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sxx.yfazqb.com

[Q74] 强制使用索引
来源：http://irw.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dbo.xuetiantiany.cn

[Q75] 日期格式化
来源：http://dqt.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wyq.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cdd.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://sjr.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cmh.sjlbkw.cn

[Q77] 时间加减
来源：http://hls.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ylo.fanxiaobao.xyz

[Q78] 当前时间
来源：http://mmh.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rye.hcnkem.com

[Q79] 字符串拼接
来源：http://xdu.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iwu.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://tvp.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://brz.jlsjyb.cn

[Q81] 字符串替换
来源：http://sns.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jfa.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://vwc.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qdq.zhoulong.xyz

[Q83] 大小写转换
来源：http://xee.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ebp.cheryme.top

[Q84] 去除首尾空格
来源：http://niw.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://gtz.tianlin.xyz

[Q85] 数值取整
来源：http://bgd.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cbp.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://ffp.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oyr.gogol.net.cn

[Q87] JSON 字段做条件
来源：http://ssm.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pku.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://wvx.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dsl.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xvd.jyoumei.cn

[Q89] 判断表是否存在
来源：http://kxt.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hih.zhaomingkeji.xyz

[Q90] 生成序号列
来源：http://thb.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yuo.yueranfly.top

================================================================================
来源：http://awr.smart0.xyz

R. Bash 专题
来源：http://nkk.yvedp.cn

================================================================================
来源：http://qqw.sxryk.cn

[R01] shebang 与严格模式
来源：http://udt.zycfv.cn

#!/usr/bin/env bash
来源：http://nba.hammf.cn

set -euo pipefail
来源：http://yzf.birdmap.top

[R02] 变量赋值与使用
来源：http://whu.jianghu66.top

name="Tom"; echo "$name"
来源：http://ykx.chenlongwang.top

[R03] 只读变量
来源：http://bxa.jinqigufen.top

readonly PI=3.14
来源：http://xiu.guowangkeji.top

[R04] 位置参数
来源：http://tms.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oem.andypj.xyz

[R05] 参数默认值
来源：http://cbt.yonumen.top

name="${1:-default}"
来源：http://uap.hnqzz.top

[R06] 判断命令是否存在
来源：http://vcp.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zvy.fanxiaobao.xyz

[R07] if 判断文件
来源：http://kco.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cnu.bbcook.cn

[R08] 数值比较
来源：http://bfn.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pjx.ppjwa.cn

[R09] 字符串比较
来源：http://dst.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nxb.fehbvm.com

[R10] 正则匹配
来源：http://hsi.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bjj.smart0.xyz

[R11] case 多分支
来源：http://imk.jinghuilouyu.cn

case "$1" in
来源：http://nes.xinyue.icu

start) echo "启动" ;;
来源：http://azq.zdqjudy.top

stop)  echo "停止" ;;
来源：http://rvf.smart0.xyz

*)     echo "未知命令" ;;
来源：http://vdn.meibo888.top

esac
来源：http://jsa.wangdashe.top

[R12] for 遍历文件
来源：http://tuw.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://hrf.daxiang520.top

[R13] for 计数循环
来源：http://qiq.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://glx.hammf.cn

[R14] C 风格 for
来源：http://bvq.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lwo.kuanghao11.cn

[R15] while 逐行读文件
来源：http://yid.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://afs.svipenyu.cn

[R16] until 等待条件
来源：http://cpm.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wyt.jyoumei.cn

[R17] 数组定义与取值
来源：http://css.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://oco.jinqigfzy.top

[R18] 遍历数组
来源：http://qee.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wcw.zhongyouzk.top

[R19] 数组长度
来源：http://ocv.chenlongwang.top

echo "${#arr[@]}"
来源：http://jkz.bbcook.cn

[R20] 关联数组（字典）
来源：http://gmy.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jxl.sjlbkw.cn

[R21] 字符串长度
来源：http://qnn.bbcook.cn

echo "${#s}"
来源：http://uft.zhaomingkeji.xyz

[R22] 截取子串
来源：http://jbd.zhongyouzk.top

echo "${s:0:5}"
来源：http://kis.hongshengwenyu.top

[R23] 字符串替换
来源：http://sdc.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gdt.hnxiangtu.top

[R24] 大小写转换
来源：http://csm.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uxo.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://upn.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ugc.dashuyun.cn

[R26] 命令替换
来源：http://rxs.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://cic.shangyingyoupin.top

[R27] 算术展开
来源：http://kzr.yj202588.top

echo $((1 + 2 * 3))
来源：http://aqm.jinqigufen.top

[R28] 浮点运算
来源：http://eyk.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://xme.bjfxy.top

[R29] 定义函数
来源：http://ixu.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhl.xinyue.icu

[R30] 函数返回状态码
来源：http://jms.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://nlr.ehwqpu.com

[R31] 局部变量
来源：http://roz.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://xgm.mhx1999.top

[R32] 参数个数校验
来源：http://qql.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ovc.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://vfh.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfk.chenlongwang.top

[R34] 退出时清理
来源：http://krt.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://dgl.jinqigufen.top

[R35] 后台执行并等待
来源：http://gqm.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gwi.yj20258.top

[R36] 并发执行多个任务
来源：http://hcl.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://txe.sufxvd.cn

[R37] 把输出赋给变量
来源：http://tep.cashguo.top

files=$(ls -1)
来源：http://xln.tianlin.xyz

[R38] 管道串联
来源：http://hty.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://wtj.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://kyi.jinqigufen.top

cmd > out.log 2>&1
来源：http://zmh.fzhhl.top

[R40] 追加写日志
来源：http://zhc.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://ncw.tarul.cn

[R41] 丢弃输出
来源：http://fzq.iojbl.cn

cmd >/dev/null 2>&1
来源：http://eyv.shuidangran.top

[R42] 输入重定向
来源：http://aua.jqgfzy.top

wc -l < a.txt
来源：http://dmh.cheryme.top

[R43] 按名字查找文件
来源：http://htj.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://ntn.cucudq.cn

[R44] 按修改时间查找
来源：http://osu.svipenyu.cn

find . -mtime -7 -type f
来源：http://gsk.ydzc1.top

[R45] 批量删除
来源：http://mtr.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://spk.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://wkw.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oms.hesvh.cn

[R47] sed 单行替换
来源：http://zfn.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://fle.zhixingplan.top

[R48] awk 取指定列
来源：http://bec.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://bnb.sjlbkw.cn

[R49] awk 带条件
来源：http://dcr.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mbe.yongpay.top

[R50] awk 求和
来源：http://swi.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://rqo.nanxuanxn.top

[R51] 排序去重取前几
来源：http://coc.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nci.hfpthk.cn

[R52] 统计行数
来源：http://fry.ivvv.top

wc -l a.txt
来源：http://qrp.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://ooj.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ppu.chenzaomai.com

[R54] 比较两个文件
来源：http://tqh.hysaishi.cn

diff a.txt b.txt
来源：http://aut.ydzc1.top

[R55] 压缩与解压
来源：http://zyl.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dkl.andypj.xyz

[R56] 远程拷贝
来源：http://ksm.316326.xyz

scp file user@host:/path/
来源：http://qjf.hammf.cn

[R57] 远程执行命令
来源：http://pdt.jiagoushi.top

ssh user@host 'uptime'
来源：http://ncp.nanxinkj.top

[R58] 下载文件
来源：http://xxd.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vey.xziqi.cn

[R59] 发 POST JSON
来源：http://jry.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fsx.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://nci.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vqe.tian-w.cn

[R61] 磁盘占用
来源：http://geb.yj20258888.top

df -h;  du -sh *
来源：http://tgq.birdmap.top

[R62] 找最占空间的文件
来源：http://hmk.yonumen.top

du -ah . | sort -rh | head -10
来源：http://jqi.tarul.cn

[R63] 内存与进程
来源：http://eqw.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://grb.jlsjyb.cn

[R64] 结束进程
来源：http://vpa.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://era.cdnleiting.top

[R65] 查看端口占用
来源：http://bwb.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pir.zhixingplan.top

[R66] 定时任务
来源：http://kem.tarul.cn

crontab -e;  crontab -l
来源：http://ktm.meibo888.top

[R67] 生成随机十六进制串
来源：http://tbi.tanke756.top

openssl rand -hex 16
来源：http://lvd.hysaishi.cn

[R68] 计算文件校验值
来源：http://nqy.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://cse.hfpthk.cn

[R69] 生成随机密码
来源：http://eef.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://whr.jinqigfzy.top

[R70] 时间戳与互转
来源：http://iio.yj202588.top

date +%s;  date -d @1700000000
来源：http://uxa.hammf.cn

[R71] 日期格式化
来源：http://mom.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqo.yangfankeji.com

[R72] 等待端口就绪
来源：http://vxv.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://poo.jianghu66.top

[R73] 分割大日志
来源：http://nxu.0kj1m.cn

split -l 1000 big.log part_
来源：http://uwm.wangshuangyany.cn

[R74] 批量重命名
来源：http://edq.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jzd.cdnleiting.top

[R75] 导出环境变量
来源：http://fsa.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://nko.wangdashe.top

[R76] 使用临时文件
来源：http://siq.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wyf.ppjwa.cn

[R77] 读取用户输入
来源：http://hti.guannengcc.top

read -rp "请输入: " ans
来源：http://wcf.zycfv.cn

[R78] 交互式菜单
来源：http://uxe.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xcx.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://wkh.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abp.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://gfw.zdqjudy.top

time ./run.sh
来源：http://sqg.xingfuxueyuan.xyz

================================================================================
来源：http://mhk.chenzaomai.com

S. C / C++ 专题
来源：http://hyd.chenjidiqi.icu

================================================================================
来源：http://xgq.hfpthk.cn

[S01] C：Hello World
来源：http://psv.fzhhl.top

#include <stdio.h>
来源：http://qvd.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ysb.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://qly.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://qkw.fzhhl.top

[S03] C：读入整数
来源：http://eoe.svipenyu.cn

int x; scanf("%d", &x);
来源：http://mik.hongshengwenyu.top

[S04] C：字符串复制
来源：http://xtn.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yuo.yuxming.cn

[S05] C：字符串长度
来源：http://abj.xylfe.cn

strlen(s)
来源：http://doa.yfazqb.com

[S06] C：字符串比较
来源：http://wqo.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://ldk.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://khr.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vka.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://mks.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qgv.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://lvr.xylfe.cn


<!-- 参考信息 -->