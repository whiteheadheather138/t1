代发 wailian999

[Q44] IN 子查询
来源：http://rid.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sas.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://kwk.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dct.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://awy.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kfp.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://wzk.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cbx.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://kdb.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gub.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://yvm.c1oappe.top

[Q49] 更新单行
来源：http://sud.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mbq.wangshuangyany.cn

[Q50] 批量更新
来源：http://wtr.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vim.yonumen.top

[Q51] 用子查询更新
来源：http://ofg.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://emx.birdmap.top

[Q52] 删除指定行
来源：http://pud.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://xdl.hesvh.cn

[Q53] 按条件删除
来源：http://mao.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://llr.svipenyu.cn

[Q54] 清空表
来源：http://lyd.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://swv.aizwys.cn

[Q55] 排名（并列占位）
来源：http://psz.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gyj.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://jrq.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dvn.meibo888.top

[Q57] 行号
来源：http://ddv.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rji.yfazqb.com

[Q58] 累计求和
来源：http://kiy.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bzv.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://cys.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ztg.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://zby.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wfd.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iqr.sufxvd.cn

[Q61] 移动平均
来源：http://hnm.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dfr.jiagoushi.top

[Q62] 分组占比
来源：http://dkv.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxo.hcnkem.com

[Q63] 开启事务
来源：http://stf.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://elh.yangfankeji.com

[Q64] 提交事务
来源：http://cod.xingfuxueyuan.xyz

COMMIT;
来源：http://isl.bjfxy.top

[Q65] 回滚事务
来源：http://zil.yj20258888.top

ROLLBACK;
来源：http://bog.havefunace.top

[Q66] 行锁查询
来源：http://vyq.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bma.ehwqpu.com

[Q67] 设置隔离级别
来源：http://pxd.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cpg.pycfn.com

[Q68] 保存点
来源：http://eyb.hnqzz.top

SAVEPOINT sp1;
来源：http://tzw.uphjek.com

ROLLBACK TO sp1;
来源：http://muj.haohaochexian.top

[Q69] 查看执行计划
来源：http://ryt.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aaj.hammf.cn

[Q70] 更新统计信息
来源：http://nlm.gaohongyu789.top

ANALYZE TABLE users;
来源：http://wyh.epnwcf.com

[Q71] 查看建表语句
来源：http://idr.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vmh.tian-w.cn

[Q72] 查看索引
来源：http://nss.uphjek.com

SHOW INDEX FROM users;
来源：http://tbp.xuetiantiany.cn

[Q73] 查看表状态
来源：http://yfz.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bmg.ehwqpu.com

[Q74] 强制使用索引
来源：http://hxl.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://odl.yj20258.top

[Q75] 日期格式化
来源：http://yqg.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dms.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rlz.zhixingplan.top

[Q76] 按天统计
来源：http://ivs.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nst.tarul.cn

[Q77] 时间加减
来源：http://jfe.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qqc.guannengcc.top

[Q78] 当前时间
来源：http://zei.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xlu.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://tsz.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nyz.cucudq.cn

[Q80] 字符串截取
来源：http://ejw.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ega.jqgufenzy.top

[Q81] 字符串替换
来源：http://gua.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iie.havefunace.top

[Q82] 字符长度与字节长度
来源：http://vur.cheryme.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yih.cdnleiting.top

[Q83] 大小写转换
来源：http://hza.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zpi.cheryme.top

[Q84] 去除首尾空格
来源：http://tir.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://wyo.redwolf501.top

[Q85] 数值取整
来源：http://nqh.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fbg.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://vot.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vec.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://zji.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pdw.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://mql.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iyb.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ahs.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://rur.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qca.gaohongyu789.top

[Q90] 生成序号列
来源：http://vux.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://otl.nanxinkj.top

================================================================================
来源：http://ade.hfpthk.cn

R. Bash 专题
来源：http://sql.ywan-chungtsiang.top

================================================================================
来源：http://xbg.yueranfly.top

[R01] shebang 与严格模式
来源：http://gmv.yvedp.cn

#!/usr/bin/env bash
来源：http://awt.svipenyu.cn

set -euo pipefail
来源：http://nfi.snrcjt.cn

[R02] 变量赋值与使用
来源：http://okn.hywenlv.cn

name="Tom"; echo "$name"
来源：http://oxv.shzxlz.cn

[R03] 只读变量
来源：http://swm.zycfv.cn

readonly PI=3.14
来源：http://ekz.yuanzhike.top

[R04] 位置参数
来源：http://fyz.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jju.xinyue.icu

[R05] 参数默认值
来源：http://ple.zhoulong.xyz

name="${1:-default}"
来源：http://wjs.ehwqpu.com

[R06] 判断命令是否存在
来源：http://asg.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ptg.tanke756.top

[R07] if 判断文件
来源：http://ebb.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ntm.xylfe.cn

[R08] 数值比较
来源：http://ydt.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gig.cucudq.cn

[R09] 字符串比较
来源：http://hkz.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ruk.chenjidiqi.icu

[R10] 正则匹配
来源：http://lxb.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pus.yongpay.top

[R11] case 多分支
来源：http://uci.sjlbkw.cn

case "$1" in
来源：http://ncm.yj202588.top

start) echo "启动" ;;
来源：http://xwh.cheryme.top

stop)  echo "停止" ;;
来源：http://rzb.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://nxb.svipenyu.cn

esac
来源：http://vix.shangyingyoupin.top

[R12] for 遍历文件
来源：http://hwf.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://yum.vehdjk.com

[R13] for 计数循环
来源：http://qbs.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://vog.dashuyun.cn

[R14] C 风格 for
来源：http://qvn.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ijr.aibaodan.cn

[R15] while 逐行读文件
来源：http://jbb.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://avx.ydzc1.top

[R16] until 等待条件
来源：http://cly.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xua.shuidangran.top

[R17] 数组定义与取值
来源：http://nii.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://xjz.uphjek.com

[R18] 遍历数组
来源：http://jkx.bjfxy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://snm.yueranfly.top

[R19] 数组长度
来源：http://igw.sweek.top

echo "${#arr[@]}"
来源：http://jkr.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://khn.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pea.haohaochexian.top

[R21] 字符串长度
来源：http://blb.mhx1999.top

echo "${#s}"
来源：http://nrg.hnxiangtu.top

[R22] 截取子串
来源：http://obq.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://iiw.yueranfly.top

[R23] 字符串替换
来源：http://ewc.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cks.0kj1m.cn

[R24] 大小写转换
来源：http://jtg.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://kug.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://cae.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rsy.dashuyun.cn

[R26] 命令替换
来源：http://xcg.yj20258.top

now=$(date +%F); echo "$now"
来源：http://pkg.nanxinkj.top

[R27] 算术展开
来源：http://gif.yueranfly.top

echo $((1 + 2 * 3))
来源：http://apj.ydzc1.top

[R28] 浮点运算
来源：http://uuc.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://eep.hammf.cn

[R29] 定义函数
来源：http://ypn.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dpv.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://yzd.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://ukq.hesvh.cn

[R31] 局部变量
来源：http://trj.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://eih.haohaochexian.top

[R32] 参数个数校验
来源：http://uhs.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcj.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://eqx.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dyb.vehdjk.com

[R34] 退出时清理
来源：http://lei.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://tcy.hnqzz.top

[R35] 后台执行并等待
来源：http://axx.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://gmd.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://icg.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://twt.hysaishi.cn

[R37] 把输出赋给变量
来源：http://fzt.jinqigfzy.top

files=$(ls -1)
来源：http://ujw.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://cso.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://xwk.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://zxt.hywenlv.cn

cmd > out.log 2>&1
来源：http://axl.feifeiyinyue.top

[R40] 追加写日志
来源：http://pqp.smart0.xyz

echo "log" >> out.log
来源：http://xzo.cucudq.cn

[R41] 丢弃输出
来源：http://mex.c1oappe.top

cmd >/dev/null 2>&1
来源：http://kbh.tanke756.top

[R42] 输入重定向
来源：http://cac.nanxinkj.top

wc -l < a.txt
来源：http://mfe.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://pgk.hcnkem.com

find . -name "*.log" -type f
来源：http://wcz.meibo888.top

[R44] 按修改时间查找
来源：http://kxn.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://jwj.yvedp.cn

[R45] 批量删除
来源：http://ykx.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://gkz.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://jtu.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tpm.daxiang520.top

[R47] sed 单行替换
来源：http://ruz.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aob.jyoumei.cn

[R48] awk 取指定列
来源：http://hor.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://unq.hesvh.cn

[R49] awk 带条件
来源：http://wgk.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lkr.jianghu66.top

[R50] awk 求和
来源：http://kpz.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://juy.gaohongyu789.top

[R51] 排序去重取前几
来源：http://flp.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nvz.yfazqb.com

[R52] 统计行数
来源：http://nfx.xylfe.cn

wc -l a.txt
来源：http://odv.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://mlq.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uzw.jyoumei.cn

[R54] 比较两个文件
来源：http://sun.shangyingyoupin.top

diff a.txt b.txt
来源：http://uyt.vehdjk.com

[R55] 压缩与解压
来源：http://ezk.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jta.yvedp.cn

[R56] 远程拷贝
来源：http://qph.xylfe.cn

scp file user@host:/path/
来源：http://klx.sjlbkw.cn

[R57] 远程执行命令
来源：http://ubc.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://rfh.vehdjk.com

[R58] 下载文件
来源：http://sse.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oeu.uphjek.com

[R59] 发 POST JSON
来源：http://cdf.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://moy.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://pfr.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://laf.haohaochexian.top

[R61] 磁盘占用
来源：http://nsi.dashuyun.cn

df -h;  du -sh *
来源：http://krx.haohaochexian.top

[R62] 找最占空间的文件
来源：http://szj.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://tcy.yuxming.cn

[R63] 内存与进程
来源：http://oyx.yonumen.top

free -h;  ps aux | grep nginx
来源：http://ggn.kuanghao11.cn

[R64] 结束进程
来源：http://sqx.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://zjw.yongpay.top

[R65] 查看端口占用
来源：http://eil.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eaq.guowangkeji.top

[R66] 定时任务
来源：http://teh.yuxming.cn

crontab -e;  crontab -l
来源：http://ysd.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://gbz.dashuyun.cn

openssl rand -hex 16
来源：http://lhr.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://qrl.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hwa.ivvv.top

[R69] 生成随机密码
来源：http://vvk.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://kyy.xinyue.icu

[R70] 时间戳与互转
来源：http://pma.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://zkk.wangshuangyany.cn

[R71] 日期格式化
来源：http://mwb.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lcm.tianlin.xyz

[R72] 等待端口就绪
来源：http://bev.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zvw.zhiwuduotai.top

[R73] 分割大日志
来源：http://zrt.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://nxj.nwbrower.top

[R74] 批量重命名
来源：http://ztm.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rdt.yueranfly.top

[R75] 导出环境变量
来源：http://iho.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://mtv.c1oappe.top

[R76] 使用临时文件
来源：http://jdx.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eic.zdbjq.cn

[R77] 读取用户输入
来源：http://two.chenzaomai.com

read -rp "请输入: " ans
来源：http://hfv.fktsv.cn

[R78] 交互式菜单
来源：http://ivp.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jwr.cqqwz.cn

[R79] 解析命令行选项
来源：http://yqc.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qrm.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://wva.gzhubu.top

time ./run.sh
来源：http://utv.jqgufenzy.top

================================================================================
来源：http://eax.jianghu66.top

S. C / C++ 专题
来源：http://cpx.zhijiandao.cn

================================================================================
来源：http://ipf.daxiang520.top

[S01] C：Hello World
来源：http://own.shuidangran.top

#include <stdio.h>
来源：http://app.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tgn.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://qoj.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://qwp.yuanzhike.top

[S03] C：读入整数
来源：http://xon.hysaishi.cn

int x; scanf("%d", &x);
来源：http://snz.316326.xyz

[S04] C：字符串复制
来源：http://yvm.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://opr.xylfe.cn

[S05] C：字符串长度
来源：http://vyl.guowangkeji.top

strlen(s)
来源：http://xkz.havefunace.top

[S06] C：字符串比较
来源：http://hqn.hesvh.cn

strcmp(a, b) == 0
来源：http://vnk.zhixingplan.top

[S07] C：数组遍历求和
来源：http://uvh.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://add.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://gib.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qqx.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://von.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vdh.havefunace.top

[S10] C：指针与解引用
来源：http://wwh.tian-w.cn

int *p = &a;  *p = 5;
来源：http://zxk.birdmap.top

[S11] C：逐行读文件
来源：http://sba.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://zxd.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uss.havefunace.top

fclose(f);
来源：http://svr.zdbjq.cn

[S12] C：写文件
来源：http://ngy.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vrr.mhx1999.top

[S13] C：宏定义
来源：http://lrl.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oct.hammf.cn

[S14] C：枚举
来源：http://gbz.yj20258.top


<!-- 参考信息 -->