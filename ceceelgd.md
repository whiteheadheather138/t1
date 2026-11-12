代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://mdk.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://krs.tarul.cn

[Q43] 标量子查询
来源：http://orc.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hdi.ehwqpu.com

[Q44] IN 子查询
来源：http://vng.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kvf.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://sbi.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ipk.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qof.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yya.uphjek.com

[Q47] 与平均值比较
来源：http://iqn.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://din.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://ihm.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lph.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://iwk.sxryk.cn

[Q49] 更新单行
来源：http://vqv.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hkq.chenjidiqi.icu

[Q50] 批量更新
来源：http://gha.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xvx.meibo888.top

[Q51] 用子查询更新
来源：http://kpd.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hqm.zdbjq.cn

[Q52] 删除指定行
来源：http://jhj.yfazqb.com

DELETE FROM users WHERE id = 10;
来源：http://qud.fehbvm.com

[Q53] 按条件删除
来源：http://xxq.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gig.cashguo.top

[Q54] 清空表
来源：http://uqj.hesvh.cn

TRUNCATE TABLE logs;
来源：http://vpk.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://zbp.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vdg.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://yhy.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://siw.yj202588.top

[Q57] 行号
来源：http://hfa.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aao.zdqjudy.top

[Q58] 累计求和
来源：http://rix.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vvv.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://fqo.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://veq.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://khg.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lok.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vzz.xylfe.cn

[Q61] 移动平均
来源：http://bzc.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dmt.tian-w.cn

[Q62] 分组占比
来源：http://zyq.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nnp.ppjwa.cn

[Q63] 开启事务
来源：http://ael.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://zqu.fanxiaobao.xyz

[Q64] 提交事务
来源：http://egs.fanxiaobao.xyz

COMMIT;
来源：http://iwl.sweek.top

[Q65] 回滚事务
来源：http://pcp.sysykeji.top

ROLLBACK;
来源：http://yya.bbcook.cn

[Q66] 行锁查询
来源：http://llj.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mek.xylfe.cn

[Q67] 设置隔离级别
来源：http://rne.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gly.sufxvd.cn

[Q68] 保存点
来源：http://kuy.sjlbkw.cn

SAVEPOINT sp1;
来源：http://oft.xuanzx.com

ROLLBACK TO sp1;
来源：http://gxz.52xcode.cn

[Q69] 查看执行计划
来源：http://chy.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vet.vehdjk.com

[Q70] 更新统计信息
来源：http://otn.vehdjk.com

ANALYZE TABLE users;
来源：http://lfi.daxiang520.top

[Q71] 查看建表语句
来源：http://jtq.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mbe.gaohongyu789.top

[Q72] 查看索引
来源：http://uzt.hywenlv.cn

SHOW INDEX FROM users;
来源：http://fsy.xziqi.cn

[Q73] 查看表状态
来源：http://voy.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gga.jinqigfzy.top

[Q74] 强制使用索引
来源：http://vsh.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ath.zhoulong.xyz

[Q75] 日期格式化
来源：http://fhj.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vgk.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rvv.jianghu66.top

[Q76] 按天统计
来源：http://upm.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lwe.tarul.cn

[Q77] 时间加减
来源：http://pkf.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jek.wangshuangyany.cn

[Q78] 当前时间
来源：http://qxe.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mxm.fehbvm.com

[Q79] 字符串拼接
来源：http://kvx.ehwqpu.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dmm.cashguo.top

[Q80] 字符串截取
来源：http://knm.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sjo.zhengqikj.top

[Q81] 字符串替换
来源：http://fwp.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dfm.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://ozl.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kem.ppjwa.cn

[Q83] 大小写转换
来源：http://kay.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fmq.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://azs.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://qbf.hysaishi.cn

[Q85] 数值取整
来源：http://paf.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmm.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://cqs.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sbv.xuanzx.com

[Q87] JSON 字段做条件
来源：http://uxz.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gkj.andypj.xyz

[Q88] 行转列（条件聚合）
来源：http://ztb.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xvb.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pdc.vehdjk.com

[Q89] 判断表是否存在
来源：http://jvg.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iqt.zhijiandao.cn

[Q90] 生成序号列
来源：http://bqg.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lks.sysykeji.top

================================================================================
来源：http://epl.52xcode.cn

R. Bash 专题
来源：http://sgw.kuanghao11.cn

================================================================================
来源：http://drc.tianlin.xyz

[R01] shebang 与严格模式
来源：http://ggi.sysykeji.top

#!/usr/bin/env bash
来源：http://bci.yj20258.top

set -euo pipefail
来源：http://sta.zdqjudy.top

[R02] 变量赋值与使用
来源：http://kif.dashuyun.cn

name="Tom"; echo "$name"
来源：http://qvu.snrcjt.cn

[R03] 只读变量
来源：http://kqc.cashguo.top

readonly PI=3.14
来源：http://ugn.bbcook.cn

[R04] 位置参数
来源：http://yjv.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fcp.hywenlv.cn

[R05] 参数默认值
来源：http://fyc.zhiwuduotai.top

name="${1:-default}"
来源：http://gir.yonumen.top

[R06] 判断命令是否存在
来源：http://bhu.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sqa.shangyingyoupin.top

[R07] if 判断文件
来源：http://rly.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oqx.c1oappe.top

[R08] 数值比较
来源：http://hjw.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xnk.meibo888.top

[R09] 字符串比较
来源：http://zrf.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://imx.cqqwz.cn

[R10] 正则匹配
来源：http://rgn.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xfz.andypj.xyz

[R11] case 多分支
来源：http://fhg.ybcxt.top

case "$1" in
来源：http://ykq.iojbl.cn

start) echo "启动" ;;
来源：http://siu.snrcjt.cn

stop)  echo "停止" ;;
来源：http://cfp.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://ocs.bbcook.cn

esac
来源：http://gbd.feifeiyinyue.top

[R12] for 遍历文件
来源：http://lkd.xingfuxueyuan.xyz

for f in *.txt; do echo "$f"; done
来源：http://xbe.bbcook.cn

[R13] for 计数循环
来源：http://evg.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://noj.wangdashe.top

[R14] C 风格 for
来源：http://tow.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://trt.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://qyc.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://usg.kuanghao11.cn

[R16] until 等待条件
来源：http://ouh.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hzq.zycfv.cn

[R17] 数组定义与取值
来源：http://bvf.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://djw.jinqigfzy.top

[R18] 遍历数组
来源：http://ips.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cec.tian-w.cn

[R19] 数组长度
来源：http://wsw.yfazqb.com

echo "${#arr[@]}"
来源：http://klu.dianchejie.cn

[R20] 关联数组（字典）
来源：http://yix.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iew.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://kgw.yvedp.cn

echo "${#s}"
来源：http://ytq.kuanghao11.cn

[R22] 截取子串
来源：http://ydg.ctjpmb.com

echo "${s:0:5}"
来源：http://nkl.52xcode.cn

[R23] 字符串替换
来源：http://rea.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pke.ehwqpu.com

[R24] 大小写转换
来源：http://zgg.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://lqx.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://lpg.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cct.gogol.net.cn

[R26] 命令替换
来源：http://htd.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://mpy.xuanzx.com

[R27] 算术展开
来源：http://bxd.aizwys.cn

echo $((1 + 2 * 3))
来源：http://cxw.jinqigfzy.top

[R28] 浮点运算
来源：http://ayn.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://cpt.smart0.xyz

[R29] 定义函数
来源：http://gte.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ysd.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://dxc.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hsn.tianlin.xyz

[R31] 局部变量
来源：http://oyv.hnqzz.top

f() { local x=1; echo "$x"; }
来源：http://qdp.chenzaomai.com

[R32] 参数个数校验
来源：http://kct.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mtl.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://qze.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xhg.yueranfly.top

[R34] 退出时清理
来源：http://tsh.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bfu.xylfe.cn

[R35] 后台执行并等待
来源：http://jvw.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hkh.hammf.cn

[R36] 并发执行多个任务
来源：http://bzu.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cdg.nwbrower.top

[R37] 把输出赋给变量
来源：http://yqj.cashguo.top

files=$(ls -1)
来源：http://yae.cdnleiting.top

[R38] 管道串联
来源：http://rdw.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://sbr.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://nhp.hammf.cn

cmd > out.log 2>&1
来源：http://hdc.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://pqz.aizwys.cn

echo "log" >> out.log
来源：http://ldi.chenlongwang.top

[R41] 丢弃输出
来源：http://bwz.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://rrn.bjfxy.top

[R42] 输入重定向
来源：http://pfr.daxiang520.top

wc -l < a.txt
来源：http://cqy.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://ozo.svipenyu.cn

find . -name "*.log" -type f
来源：http://rke.gotoacloud.top

[R44] 按修改时间查找
来源：http://gmk.chenlongwang.top

find . -mtime -7 -type f
来源：http://nne.tarul.cn

[R45] 批量删除
来源：http://djv.yfazqb.com

find . -name "*.tmp" -delete
来源：http://rrs.aizwys.cn

[R46] 递归替换文件内容
来源：http://waq.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tpb.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://qdz.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://ysu.zdqjudy.top

[R48] awk 取指定列
来源：http://swz.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://gtb.bjfxy.top

[R49] awk 带条件
来源：http://ios.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://skm.yuanzhike.top

[R50] awk 求和
来源：http://mly.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cnm.ydzc1.top

[R51] 排序去重取前几
来源：http://yqc.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://smr.jinyuanbaomall.cn

[R52] 统计行数
来源：http://jkk.shanyushiyangtech.top

wc -l a.txt
来源：http://pri.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://vfd.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qfd.iojbl.cn

[R54] 比较两个文件
来源：http://udw.yj20258888.top

diff a.txt b.txt
来源：http://obs.jinqigfzy.top

[R55] 压缩与解压
来源：http://nro.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uno.daria6918.cn

[R56] 远程拷贝
来源：http://evf.fktsv.cn

scp file user@host:/path/
来源：http://msi.yj202588.top

[R57] 远程执行命令
来源：http://wdl.birdmap.top

ssh user@host 'uptime'
来源：http://pnk.zycfv.cn

[R58] 下载文件
来源：http://awf.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbw.sufxvd.cn

[R59] 发 POST JSON
来源：http://qem.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lnb.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://zsh.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nrq.nanxuanxn.top

[R61] 磁盘占用
来源：http://ndb.hesvh.cn

df -h;  du -sh *
来源：http://rmd.cdnleiting.top

[R62] 找最占空间的文件
来源：http://zes.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://spn.ybcxt.top

[R63] 内存与进程
来源：http://ezu.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://pcm.birdmap.top

[R64] 结束进程
来源：http://khl.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://rfw.aizwys.cn

[R65] 查看端口占用
来源：http://cmo.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pei.tian-w.cn

[R66] 定时任务
来源：http://qtk.zhongyouzk.top

crontab -e;  crontab -l
来源：http://aql.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://rkj.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://leh.jianghu66.top

[R68] 计算文件校验值
来源：http://njz.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mal.52xcode.cn

[R69] 生成随机密码
来源：http://wib.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://ibh.bjfxy.top

[R70] 时间戳与互转
来源：http://uhj.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://rwp.gzhubu.top

[R71] 日期格式化
来源：http://fda.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://njh.fzhhl.top

[R72] 等待端口就绪
来源：http://kog.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lgz.tarul.cn

[R73] 分割大日志
来源：http://osm.daxiang520.top

split -l 1000 big.log part_
来源：http://xci.gotoacloud.top

[R74] 批量重命名
来源：http://qht.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lsc.cashguo.top

[R75] 导出环境变量
来源：http://pxs.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://jls.daria6918.cn

[R76] 使用临时文件
来源：http://nup.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://asn.haohaochexian.top

[R77] 读取用户输入
来源：http://cit.bjfxy.top

read -rp "请输入: " ans
来源：http://zok.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://rfp.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://coa.xuanzx.com

[R79] 解析命令行选项
来源：http://ztn.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gnc.hcnkem.com

[R80] 查看脚本执行耗时
来源：http://irf.jiagoushi.top

time ./run.sh
来源：http://ein.svipenyu.cn

================================================================================
来源：http://npi.meibo888.top

S. C / C++ 专题
来源：http://ifv.yueranfly.top

================================================================================
来源：http://rqc.cheryme.top

[S01] C：Hello World
来源：http://jqe.0kj1m.cn

#include <stdio.h>
来源：http://mqw.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gwr.fehbvm.com

[S02] C：变量与格式化输出
来源：http://yss.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://dkk.aibaodan.cn

[S03] C：读入整数
来源：http://vfs.cqqwz.cn

int x; scanf("%d", &x);
来源：http://wcc.zhengqikj.top

[S04] C：字符串复制
来源：http://drl.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cdj.redwolf501.top

[S05] C：字符串长度
来源：http://vaz.gzhubu.top

strlen(s)
来源：http://tti.xuetiantiany.cn

[S06] C：字符串比较
来源：http://irn.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://hhm.ppjwa.cn

[S07] C：数组遍历求和
来源：http://uta.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://arm.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://qpx.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vyu.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://oma.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fim.zhengqikj.top

[S10] C：指针与解引用
来源：http://ggh.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://itp.andypj.xyz

[S11] C：逐行读文件
来源：http://xbv.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://vcc.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nck.xuanzx.com

fclose(f);
来源：http://thj.snrcjt.cn

[S12] C：写文件
来源：http://arl.tanke756.top


<!-- 参考信息 -->