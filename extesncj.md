代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://rui.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yih.cdnleiting.top

[Q47] 与平均值比较
来源：http://okn.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xjo.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://qsc.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://maq.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://uth.xziqi.cn

[Q49] 更新单行
来源：http://fer.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aim.jinqigufen.top

[Q50] 批量更新
来源：http://jss.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qar.zdqjudy.top

[Q51] 用子查询更新
来源：http://sre.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://chy.epnwcf.com

[Q52] 删除指定行
来源：http://eau.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://aec.zhiwuduotai.top

[Q53] 按条件删除
来源：http://alh.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://klc.jinqigufen.top

[Q54] 清空表
来源：http://bmw.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://nap.bbcook.cn

[Q55] 排名（并列占位）
来源：http://wzg.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zke.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://zaw.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ena.shanyushiyangtech.top

[Q57] 行号
来源：http://eep.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://olt.ybcxt.top

[Q58] 累计求和
来源：http://cvm.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yzj.zycfv.cn

[Q59] 分组内累计
来源：http://aei.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bvs.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://nbo.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dap.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hyw.sufxvd.cn

[Q61] 移动平均
来源：http://kpx.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wzn.uphjek.com

[Q62] 分组占比
来源：http://wfm.52xcode.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zhd.yongpay.top

[Q63] 开启事务
来源：http://xvw.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://xos.uphjek.com

[Q64] 提交事务
来源：http://qyj.aibaodan.cn

COMMIT;
来源：http://jzj.ybcxt.top

[Q65] 回滚事务
来源：http://sfr.cheryme.top

ROLLBACK;
来源：http://ogz.nanxuanxn.top

[Q66] 行锁查询
来源：http://cmy.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kbz.uphjek.com

[Q67] 设置隔离级别
来源：http://isb.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://auq.tanke756.top

[Q68] 保存点
来源：http://tjs.vehdjk.com

SAVEPOINT sp1;
来源：http://dnc.shzxlz.cn

ROLLBACK TO sp1;
来源：http://ygx.pycfn.com

[Q69] 查看执行计划
来源：http://dwm.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://odm.hammf.cn

[Q70] 更新统计信息
来源：http://sbj.hesvh.cn

ANALYZE TABLE users;
来源：http://kar.52xcode.cn

[Q71] 查看建表语句
来源：http://wpv.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hot.hesvh.cn

[Q72] 查看索引
来源：http://onh.yuanzhike.top

SHOW INDEX FROM users;
来源：http://rgr.dashuyun.cn

[Q73] 查看表状态
来源：http://vwk.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://swa.gogol.net.cn

[Q74] 强制使用索引
来源：http://gia.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eze.fktsv.cn

[Q75] 日期格式化
来源：http://kpa.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ihy.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fzk.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://iuk.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jjc.tianlin.xyz

[Q77] 时间加减
来源：http://yha.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wlu.dashuyun.cn

[Q78] 当前时间
来源：http://vcw.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vrc.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://utb.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://grt.vqdsnc.cn

[Q80] 字符串截取
来源：http://lal.ydjk.org.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cyi.cashguo.top

[Q81] 字符串替换
来源：http://elf.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yqo.fzhhl.top

[Q82] 字符长度与字节长度
来源：http://zjd.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://khj.fzhhl.top

[Q83] 大小写转换
来源：http://nzm.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vur.iojbl.cn

[Q84] 去除首尾空格
来源：http://wre.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://gwr.yj20258.top

[Q85] 数值取整
来源：http://zdq.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lrt.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://fff.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vmt.hcnkem.com

[Q87] JSON 字段做条件
来源：http://vpv.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pam.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://vnc.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://alt.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lmd.fktsv.cn

[Q89] 判断表是否存在
来源：http://caf.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tqb.chenlongwang.top

[Q90] 生成序号列
来源：http://eqc.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvs.dashuyun.cn

================================================================================
来源：http://jno.yuxming.cn

R. Bash 专题
来源：http://tmw.shuidangran.top

================================================================================
来源：http://frh.cqqwz.cn

[R01] shebang 与严格模式
来源：http://soi.dianchejie.cn

#!/usr/bin/env bash
来源：http://tdq.9152youxi.cn

set -euo pipefail
来源：http://bik.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://tij.tanke756.top

name="Tom"; echo "$name"
来源：http://lku.chenlongwang.top

[R03] 只读变量
来源：http://hyp.uphjek.com

readonly PI=3.14
来源：http://tye.sysykeji.top

[R04] 位置参数
来源：http://ack.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bnl.xziqi.cn

[R05] 参数默认值
来源：http://uig.ppjwa.cn

name="${1:-default}"
来源：http://mrp.bbcook.cn

[R06] 判断命令是否存在
来源：http://izr.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bpc.quarkkingdee.top

[R07] if 判断文件
来源：http://dxo.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nsi.jiagoushi.top

[R08] 数值比较
来源：http://xic.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://iez.daxiang520.top

[R09] 字符串比较
来源：http://kmm.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vmm.fengsongda.top

[R10] 正则匹配
来源：http://qds.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mgy.shuidangran.top

[R11] case 多分支
来源：http://vmn.bbcook.cn

case "$1" in
来源：http://vbm.ctjpmb.com

start) echo "启动" ;;
来源：http://cmr.yuanzhike.top

stop)  echo "停止" ;;
来源：http://ejp.ydzc1.top

*)     echo "未知命令" ;;
来源：http://ois.shanyushiyangkeji.top

esac
来源：http://rcy.zhiwuduotai.top

[R12] for 遍历文件
来源：http://vqm.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://onu.jiagoushi.top

[R13] for 计数循环
来源：http://tps.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://gav.yj202588.top

[R14] C 风格 for
来源：http://eet.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bre.yuanzhike.top

[R15] while 逐行读文件
来源：http://wau.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qwa.yanxiufei.cn

[R16] until 等待条件
来源：http://ifo.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mhx.birdmap.top

[R17] 数组定义与取值
来源：http://prm.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://liq.ehwqpu.com

[R18] 遍历数组
来源：http://zad.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dok.hysaishi.cn

[R19] 数组长度
来源：http://kry.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://eix.nanxinkj.top

[R20] 关联数组（字典）
来源：http://dum.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gmi.ctjpmb.com

[R21] 字符串长度
来源：http://pjw.chenlongwang.top

echo "${#s}"
来源：http://wyo.hammf.cn

[R22] 截取子串
来源：http://pgf.hammf.cn

echo "${s:0:5}"
来源：http://dug.mhx1999.top

[R23] 字符串替换
来源：http://gvc.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mmm.xuetiantiany.cn

[R24] 大小写转换
来源：http://yvw.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://jci.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://pnb.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://eva.xuetiantiany.cn

[R26] 命令替换
来源：http://knw.uphjek.com

now=$(date +%F); echo "$now"
来源：http://erp.tian-w.cn

[R27] 算术展开
来源：http://giz.pycfn.com

echo $((1 + 2 * 3))
来源：http://wqh.gotoacloud.top

[R28] 浮点运算
来源：http://gra.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://xxd.shangyingyoupin.top

[R29] 定义函数
来源：http://qxk.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://def.jinqigfzy.top

[R30] 函数返回状态码
来源：http://upd.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://nkd.ivvv.top

[R31] 局部变量
来源：http://rvl.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://cdj.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://dvi.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lqa.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://fmn.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bpu.yongpay.top

[R34] 退出时清理
来源：http://tcp.hysaishi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://teb.zhongyouzk.top

[R35] 后台执行并等待
来源：http://pwh.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gij.jqgfzy.top

[R36] 并发执行多个任务
来源：http://hrf.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://epu.aizwys.cn

[R37] 把输出赋给变量
来源：http://lcj.quarkkingdee.top

files=$(ls -1)
来源：http://hkk.yvedp.cn

[R38] 管道串联
来源：http://xnh.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://mtp.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://szd.sufxvd.cn

cmd > out.log 2>&1
来源：http://ipi.daria6918.cn

[R40] 追加写日志
来源：http://jfr.epnwcf.com

echo "log" >> out.log
来源：http://enj.tianlin.xyz

[R41] 丢弃输出
来源：http://nsg.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://dso.yfazqb.com

[R42] 输入重定向
来源：http://ame.hnqzz.top

wc -l < a.txt
来源：http://brd.cqqwz.cn

[R43] 按名字查找文件
来源：http://nue.uphjek.com

find . -name "*.log" -type f
来源：http://tjy.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://puy.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://tpe.yuxming.cn

[R45] 批量删除
来源：http://grh.c1oappe.top

find . -name "*.tmp" -delete
来源：http://dpf.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://zef.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xla.yueranfly.top

[R47] sed 单行替换
来源：http://gfr.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aki.ctjpmb.com

[R48] awk 取指定列
来源：http://sep.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://jxr.shangyingyoupin.top

[R49] awk 带条件
来源：http://zsc.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avc.jianghu66.top

[R50] awk 求和
来源：http://aeu.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://mob.ydzc1.top

[R51] 排序去重取前几
来源：http://llq.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rsc.hnxiangtu.top

[R52] 统计行数
来源：http://dqz.chenlongwang.top

wc -l a.txt
来源：http://agb.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://lsq.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pti.mhx1999.top

[R54] 比较两个文件
来源：http://kzd.birdmap.top

diff a.txt b.txt
来源：http://rgv.jqgufenzy.top

[R55] 压缩与解压
来源：http://mey.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wxn.sufxvd.cn

[R56] 远程拷贝
来源：http://jsj.mhx1999.top

scp file user@host:/path/
来源：http://pjv.wangshuangyany.cn

[R57] 远程执行命令
来源：http://ufv.guowangkeji.top

ssh user@host 'uptime'
来源：http://zjc.jiagoushi.top

[R58] 下载文件
来源：http://goa.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bxf.epnwcf.com

[R59] 发 POST JSON
来源：http://owe.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rwx.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://boo.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uxa.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://dyg.xylfe.cn

df -h;  du -sh *
来源：http://pbd.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://ccx.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://tfe.yj20258.top

[R63] 内存与进程
来源：http://irt.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://smk.fengsongda.top

[R64] 结束进程
来源：http://vuu.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://cnw.zhixingplan.top

[R65] 查看端口占用
来源：http://mze.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqm.xziqi.cn

[R66] 定时任务
来源：http://vua.hfpthk.cn

crontab -e;  crontab -l
来源：http://kae.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://gtm.sufxvd.cn

openssl rand -hex 16
来源：http://gde.andypj.xyz

[R68] 计算文件校验值
来源：http://myx.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gmo.sweek.top

[R69] 生成随机密码
来源：http://rsv.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://rpr.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://onb.xinyue.icu

date +%s;  date -d @1700000000
来源：http://ese.sweek.top

[R71] 日期格式化
来源：http://ffz.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ird.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://lwo.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hil.yj202588.top

[R73] 分割大日志
来源：http://qop.tarul.cn

split -l 1000 big.log part_
来源：http://vfw.hysaishi.cn

[R74] 批量重命名
来源：http://vla.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fas.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://dys.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://vkm.cqqwz.cn

[R76] 使用临时文件
来源：http://ldw.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://odk.ydjk.org.cn

[R77] 读取用户输入
来源：http://hgc.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://dsg.zhixingplan.top

[R78] 交互式菜单
来源：http://wxv.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fdg.yueranfly.top

[R79] 解析命令行选项
来源：http://jze.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uaz.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://jwc.snrcjt.cn

time ./run.sh
来源：http://pha.zhoulong.xyz

================================================================================
来源：http://bzt.chenlongwang.top

S. C / C++ 专题
来源：http://jki.cucudq.cn

================================================================================
来源：http://lrt.feifeiyinyue.top

[S01] C：Hello World
来源：http://kgj.bbcook.cn

#include <stdio.h>
来源：http://mga.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hzn.yfazqb.com

[S02] C：变量与格式化输出
来源：http://wbf.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://guq.chenlongwang.top

[S03] C：读入整数
来源：http://vsy.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://mvn.daxiang520.top

[S04] C：字符串复制
来源：http://hpx.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://jor.hnxiangtu.top

[S05] C：字符串长度
来源：http://qxg.gogol.net.cn

strlen(s)
来源：http://hhb.dianchejie.cn

[S06] C：字符串比较
来源：http://xhb.ydjk.org.cn

strcmp(a, b) == 0
来源：http://xpf.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://yxs.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ike.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://bsh.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qdw.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://jtg.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://odd.shzxlz.cn

[S10] C：指针与解引用
来源：http://vku.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://duq.meibo888.top

[S11] C：逐行读文件
来源：http://cdu.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://pwg.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://prs.hysaishi.cn

fclose(f);
来源：http://cpo.chenlongwang.top

[S12] C：写文件
来源：http://sgn.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://evj.gzhubu.top

[S13] C：宏定义
来源：http://jxv.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gge.sweek.top

[S14] C：枚举
来源：http://oau.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://dcj.uphjek.com

[S15] C：类型转换
来源：http://gnk.smart0.xyz

(double) a / b
来源：http://yql.sjlbkw.cn

[S16] C：位操作置位
来源：http://mse.hfpthk.cn


<!-- 参考信息 -->