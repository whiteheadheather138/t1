代发 wailian999

[Q44] IN 子查询
来源：http://moy.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zdt.316326.xyz

[Q45] EXISTS 判断存在
来源：http://rns.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pih.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ivn.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkc.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://fvm.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ohe.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://yts.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://efc.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://oly.fzhhl.top

[Q49] 更新单行
来源：http://ted.gogol.net.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nds.hongshengwenyu.top

[Q50] 批量更新
来源：http://lap.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lqk.wangdashe.top

[Q51] 用子查询更新
来源：http://maf.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zry.zdqjudy.top

[Q52] 删除指定行
来源：http://dnu.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://glg.fanxiaobao.xyz

[Q53] 按条件删除
来源：http://jwv.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mkj.ppjwa.cn

[Q54] 清空表
来源：http://guk.hcnkem.com

TRUNCATE TABLE logs;
来源：http://gsw.yonumen.top

[Q55] 排名（并列占位）
来源：http://svr.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gxu.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://jhy.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wye.jinghuilouyu.cn

[Q57] 行号
来源：http://dwn.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fqu.zhengqikj.top

[Q58] 累计求和
来源：http://vxl.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qgd.shangyingyoupin.top

[Q59] 分组内累计
来源：http://mtw.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bbb.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://azi.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sne.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hts.tianlin.xyz

[Q61] 移动平均
来源：http://vof.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uji.svipenyu.cn

[Q62] 分组占比
来源：http://hjw.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jaj.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://hmj.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://frj.havefunace.top

[Q64] 提交事务
来源：http://rnx.zdqjudy.top

COMMIT;
来源：http://bqy.ydzc1.top

[Q65] 回滚事务
来源：http://asg.ivvv.top

ROLLBACK;
来源：http://mzm.zhongyouzk.top

[Q66] 行锁查询
来源：http://ang.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://skf.xuanzx.com

[Q67] 设置隔离级别
来源：http://rmt.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hds.ydjk.org.cn

[Q68] 保存点
来源：http://poe.snrcjt.cn

SAVEPOINT sp1;
来源：http://aii.316326.xyz

ROLLBACK TO sp1;
来源：http://efs.yj20258888.top

[Q69] 查看执行计划
来源：http://fty.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ydo.hammf.cn

[Q70] 更新统计信息
来源：http://cxk.hfpthk.cn

ANALYZE TABLE users;
来源：http://hmt.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://mem.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fjz.meibo888.top

[Q72] 查看索引
来源：http://utz.sweek.top

SHOW INDEX FROM users;
来源：http://nis.tanke756.top

[Q73] 查看表状态
来源：http://bri.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iow.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://lrd.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://geo.0kj1m.cn

[Q75] 日期格式化
来源：http://jfh.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gnr.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ayo.yvedp.cn

[Q76] 按天统计
来源：http://dul.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hkg.tanke756.top

[Q77] 时间加减
来源：http://ere.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hjw.jiagoushi.top

[Q78] 当前时间
来源：http://kiq.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zcq.zhijiandao.cn

[Q79] 字符串拼接
来源：http://rqp.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://trx.dianchejie.cn

[Q80] 字符串截取
来源：http://ksy.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iwj.zhiwuduotai.top

[Q81] 字符串替换
来源：http://jxj.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vhu.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://ivr.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aje.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://vqg.tian-w.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oil.uphjek.com

[Q84] 去除首尾空格
来源：http://uos.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://hpb.vqdsnc.cn

[Q85] 数值取整
来源：http://wuz.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qgl.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://yax.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lcp.nwbrower.top

[Q87] JSON 字段做条件
来源：http://sxr.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://laq.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://skm.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lji.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qui.epnwcf.com

[Q89] 判断表是否存在
来源：http://sni.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wjo.vehdjk.com

[Q90] 生成序号列
来源：http://lkn.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nxz.jinqigufen.top

================================================================================
来源：http://lhj.vqdsnc.cn

R. Bash 专题
来源：http://fxo.fengsongda.top

================================================================================
来源：http://dap.nanxinkj.top

[R01] shebang 与严格模式
来源：http://vee.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://yri.ybcxt.top

set -euo pipefail
来源：http://lqq.ybcxt.top

[R02] 变量赋值与使用
来源：http://fjo.yfazqb.com

name="Tom"; echo "$name"
来源：http://hco.sweek.top

[R03] 只读变量
来源：http://dvv.c1oappe.top

readonly PI=3.14
来源：http://ykq.shuidangran.top

[R04] 位置参数
来源：http://onv.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gce.ydzc1.top

[R05] 参数默认值
来源：http://mmc.yanxiufei.cn

name="${1:-default}"
来源：http://xxn.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://gxs.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cer.andypj.xyz

[R07] if 判断文件
来源：http://ffc.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgm.dianchejie.cn

[R08] 数值比较
来源：http://isb.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iaa.daxiang520.top

[R09] 字符串比较
来源：http://qxx.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ate.sysykeji.top

[R10] 正则匹配
来源：http://ecg.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://erq.uphjek.com

[R11] case 多分支
来源：http://ucd.jiagoushi.top

case "$1" in
来源：http://sfc.chenlongwang.top

start) echo "启动" ;;
来源：http://veh.zhixingplan.top

stop)  echo "停止" ;;
来源：http://gzi.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://htz.uphjek.com

esac
来源：http://ycy.dianchejie.cn

[R12] for 遍历文件
来源：http://gyw.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://apx.ppjwa.cn

[R13] for 计数循环
来源：http://bhe.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://eks.hongshengwenyu.top

[R14] C 风格 for
来源：http://rii.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dvw.yonumen.top

[R15] while 逐行读文件
来源：http://csb.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qar.jqgufenzy.top

[R16] until 等待条件
来源：http://sjz.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ush.yj20258.top

[R17] 数组定义与取值
来源：http://pwh.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://arr.bbcook.cn

[R18] 遍历数组
来源：http://txs.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xpl.xylfe.cn

[R19] 数组长度
来源：http://nwo.uphjek.com

echo "${#arr[@]}"
来源：http://ujk.yueranfly.top

[R20] 关联数组（字典）
来源：http://xky.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jjy.zdbjq.cn

[R21] 字符串长度
来源：http://toz.jinqigfzy.top

echo "${#s}"
来源：http://zrs.daxiang520.top

[R22] 截取子串
来源：http://ula.fengsongda.top

echo "${s:0:5}"
来源：http://yos.chenzaomai.com

[R23] 字符串替换
来源：http://xij.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jvc.shzxlz.cn

[R24] 大小写转换
来源：http://dxk.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://vya.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://bni.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bxt.pengpengdd.cyou

[R26] 命令替换
来源：http://xea.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://nwi.gotoacloud.top

[R27] 算术展开
来源：http://geu.yj20258888.top

echo $((1 + 2 * 3))
来源：http://var.zhijiandao.cn

[R28] 浮点运算
来源：http://xby.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://lxt.zdbjq.cn

[R29] 定义函数
来源：http://jsr.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ncp.jinqigfzy.top

[R30] 函数返回状态码
来源：http://ilt.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://srw.shzxlz.cn

[R31] 局部变量
来源：http://ale.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://kkx.c1oappe.top

[R32] 参数个数校验
来源：http://vda.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nzt.hammf.cn

[R33] 捕获错误并提示行号
来源：http://kzp.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ajy.chenzaomai.com

[R34] 退出时清理
来源：http://uol.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kzn.yj202588.top

[R35] 后台执行并等待
来源：http://jph.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vzn.yj20258.top

[R36] 并发执行多个任务
来源：http://wlo.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vft.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://doo.yangfankeji.com

files=$(ls -1)
来源：http://ljr.epnwcf.com

[R38] 管道串联
来源：http://yfb.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://roh.cashguo.top

[R39] 重定向标准输出与错误
来源：http://zch.ppjwa.cn

cmd > out.log 2>&1
来源：http://hcw.zhiwuduotai.top

[R40] 追加写日志
来源：http://efa.yongpay.top

echo "log" >> out.log
来源：http://jwx.wangshuangyany.cn

[R41] 丢弃输出
来源：http://bjk.daxiang520.top

cmd >/dev/null 2>&1
来源：http://ldu.zhengqikj.top

[R42] 输入重定向
来源：http://fpi.guowangkeji.top

wc -l < a.txt
来源：http://kvs.hywenlv.cn

[R43] 按名字查找文件
来源：http://ngn.shuidangran.top

find . -name "*.log" -type f
来源：http://xhy.nwbrower.top

[R44] 按修改时间查找
来源：http://mdt.yangfankeji.com

find . -mtime -7 -type f
来源：http://yxt.cdnleiting.top

[R45] 批量删除
来源：http://kya.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://uvd.haohaochexian.top

[R46] 递归替换文件内容
来源：http://lar.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fxu.mhx1999.top

[R47] sed 单行替换
来源：http://rjm.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fxg.xuanzx.com

[R48] awk 取指定列
来源：http://lsy.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://szi.zhongyouzk.top

[R49] awk 带条件
来源：http://tdm.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xwj.chenjidiqi.icu

[R50] awk 求和
来源：http://flh.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eqx.hcnkem.com

[R51] 排序去重取前几
来源：http://yhb.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ngl.meibo888.top

[R52] 统计行数
来源：http://yjt.tianlin.xyz

wc -l a.txt
来源：http://asg.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://jva.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fcy.havefunace.top

[R54] 比较两个文件
来源：http://yxo.hnxiangtu.top

diff a.txt b.txt
来源：http://phu.gaohongyu789.top

[R55] 压缩与解压
来源：http://sjk.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fln.gaohongyu789.top

[R56] 远程拷贝
来源：http://ize.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://oam.xuetiantiany.cn

[R57] 远程执行命令
来源：http://frs.ydzc1.top

ssh user@host 'uptime'
来源：http://dge.pycfn.com

[R58] 下载文件
来源：http://ybg.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qba.sysykeji.top

[R59] 发 POST JSON
来源：http://xyl.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://czv.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://xey.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mau.hcnkem.com

[R61] 磁盘占用
来源：http://tjs.hesvh.cn

df -h;  du -sh *
来源：http://dls.yonumen.top

[R62] 找最占空间的文件
来源：http://qkg.uphjek.com

du -ah . | sort -rh | head -10
来源：http://ywm.andypj.xyz

[R63] 内存与进程
来源：http://wjv.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://she.havefunace.top

[R64] 结束进程
来源：http://oga.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://xgp.vqdsnc.cn

[R65] 查看端口占用
来源：http://jot.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tcp.zhijiandao.cn

[R66] 定时任务
来源：http://oyo.yuanzhike.top

crontab -e;  crontab -l
来源：http://aal.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://lqa.sweek.top

openssl rand -hex 16
来源：http://unx.wangdashe.top

[R68] 计算文件校验值
来源：http://auz.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://eoq.hywenlv.cn

[R69] 生成随机密码
来源：http://gya.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://mxq.xuanzx.com

[R70] 时间戳与互转
来源：http://czm.hammf.cn

date +%s;  date -d @1700000000
来源：http://icl.316326.xyz

[R71] 日期格式化
来源：http://anq.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uyd.zhijiandao.cn

[R72] 等待端口就绪
来源：http://ybl.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xyo.cucudq.cn

[R73] 分割大日志
来源：http://qvj.jinqigfzy.top

split -l 1000 big.log part_
来源：http://iuf.vqdsnc.cn

[R74] 批量重命名
来源：http://wyf.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zrh.yfazqb.com

[R75] 导出环境变量
来源：http://yxe.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://plp.yj20258888.top

[R76] 使用临时文件
来源：http://htb.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bhr.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://vcl.sysykeji.top

read -rp "请输入: " ans
来源：http://pnh.hywenlv.cn

[R78] 交互式菜单
来源：http://axw.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qtm.zycfv.cn

[R79] 解析命令行选项
来源：http://lmk.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hst.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://puk.jqgufenzy.top

time ./run.sh
来源：http://ise.yuanzhike.top

================================================================================
来源：http://syo.feifeiyinyue.top

S. C / C++ 专题
来源：http://qwj.xuanzx.com

================================================================================
来源：http://jjl.sysykeji.top

[S01] C：Hello World
来源：http://ftl.kuanghao11.cn

#include <stdio.h>
来源：http://lrx.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uap.gzhubu.top

[S02] C：变量与格式化输出
来源：http://qzr.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://obn.yfazqb.com

[S03] C：读入整数
来源：http://qwy.shzxlz.cn

int x; scanf("%d", &x);
来源：http://rku.yueranfly.top

[S04] C：字符串复制
来源：http://jwf.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jgb.yongpay.top

[S05] C：字符串长度
来源：http://mig.smart0.xyz

strlen(s)
来源：http://ndz.haohaochexian.top

[S06] C：字符串比较
来源：http://rdr.cashguo.top

strcmp(a, b) == 0
来源：http://ajd.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://vyl.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ard.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://rsx.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iby.hammf.cn

[S09] C：结构体定义与初始化
来源：http://mft.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tft.yj20258888.top

[S10] C：指针与解引用
来源：http://nnj.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://aga.daria6918.cn

[S11] C：逐行读文件
来源：http://qxw.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://foc.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jef.yanxiufei.cn

fclose(f);
来源：http://rfl.hammf.cn

[S12] C：写文件
来源：http://mxz.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tpt.guannengcc.top

[S13] C：宏定义
来源：http://rvx.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wct.hammf.cn

[S14] C：枚举
来源：http://zcn.sysykeji.top


<!-- 参考信息 -->