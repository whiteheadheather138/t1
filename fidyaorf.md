代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zvt.andypj.xyz

[Q50] 批量更新
来源：http://gdu.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dvz.aibaodan.cn

[Q51] 用子查询更新
来源：http://qmr.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zkl.guowangkeji.top

[Q52] 删除指定行
来源：http://hde.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://ihm.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://eix.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dcc.yj202588.top

[Q54] 清空表
来源：http://iym.hesvh.cn

TRUNCATE TABLE logs;
来源：http://pvm.fktsv.cn

[Q55] 排名（并列占位）
来源：http://pjx.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzv.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://oxq.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dki.feifeiyinyue.top

[Q57] 行号
来源：http://ifu.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xmf.cdnleiting.top

[Q58] 累计求和
来源：http://grq.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jzz.daria6918.cn

[Q59] 分组内累计
来源：http://bms.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://isj.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://eqk.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nch.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csv.c1oappe.top

[Q61] 移动平均
来源：http://mpt.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ile.daria6918.cn

[Q62] 分组占比
来源：http://uue.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fll.svipenyu.cn

[Q63] 开启事务
来源：http://xim.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ymy.mhx1999.top

[Q64] 提交事务
来源：http://mxj.quarkkingdee.top

COMMIT;
来源：http://aaj.zhijiandao.cn

[Q65] 回滚事务
来源：http://grz.nwbrower.top

ROLLBACK;
来源：http://tzw.guannengcc.top

[Q66] 行锁查询
来源：http://iwy.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gta.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://ndg.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jba.shangyingyoupin.top

[Q68] 保存点
来源：http://cpr.zhoulong.xyz

SAVEPOINT sp1;
来源：http://dwe.birdmap.top

ROLLBACK TO sp1;
来源：http://wcz.zhijiandao.cn

[Q69] 查看执行计划
来源：http://bvh.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jhh.jinqigufen.top

[Q70] 更新统计信息
来源：http://daa.dashuyun.cn

ANALYZE TABLE users;
来源：http://nny.jinqigfzy.top

[Q71] 查看建表语句
来源：http://idh.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jlo.hnqzz.top

[Q72] 查看索引
来源：http://lhn.fehbvm.com

SHOW INDEX FROM users;
来源：http://iek.chenzaomai.com

[Q73] 查看表状态
来源：http://ziw.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gqr.hysaishi.cn

[Q74] 强制使用索引
来源：http://vrd.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ety.nanxuanxn.top

[Q75] 日期格式化
来源：http://toe.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tuh.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://evh.smart0.xyz

[Q76] 按天统计
来源：http://djz.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rmx.cheryme.top

[Q77] 时间加减
来源：http://qcu.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cno.yvedp.cn

[Q78] 当前时间
来源：http://hns.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vwd.yfazqb.com

[Q79] 字符串拼接
来源：http://mhc.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cio.havefunace.top

[Q80] 字符串截取
来源：http://rch.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mjo.jqgufenzy.top

[Q81] 字符串替换
来源：http://tvu.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sab.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://prt.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ocv.aibaodan.cn

[Q83] 大小写转换
来源：http://fpi.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ayo.hywenlv.cn

[Q84] 去除首尾空格
来源：http://xvs.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://tsn.guannengcc.top

[Q85] 数值取整
来源：http://qvu.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gbt.316326.xyz

[Q86] 读取 JSON 字段
来源：http://lbm.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rez.xuanzx.com

[Q87] JSON 字段做条件
来源：http://xhm.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jut.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://wyn.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jsn.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://trr.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://uef.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://phb.redwolf501.top

[Q90] 生成序号列
来源：http://ysl.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blg.jinghuilouyu.cn

================================================================================
来源：http://rqf.zycfv.cn

R. Bash 专题
来源：http://jqd.fzhhl.top

================================================================================
来源：http://xiu.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://qlx.hcnkem.com

#!/usr/bin/env bash
来源：http://fpx.gaohongyu789.top

set -euo pipefail
来源：http://vma.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://qvs.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://kyf.ybcxt.top

[R03] 只读变量
来源：http://scg.cheryme.top

readonly PI=3.14
来源：http://aqy.daria6918.cn

[R04] 位置参数
来源：http://ngm.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kzc.ybcxt.top

[R05] 参数默认值
来源：http://mfs.yueranfly.top

name="${1:-default}"
来源：http://fld.mhx1999.top

[R06] 判断命令是否存在
来源：http://hcq.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eda.yangfankeji.com

[R07] if 判断文件
来源：http://ffc.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ngu.gzhubu.top

[R08] 数值比较
来源：http://lhj.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ues.jyoumei.cn

[R09] 字符串比较
来源：http://pte.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://opu.pycfn.com

[R10] 正则匹配
来源：http://tif.aizwys.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jja.hfpthk.cn

[R11] case 多分支
来源：http://jqr.wangshuangyany.cn

case "$1" in
来源：http://imo.tarul.cn

start) echo "启动" ;;
来源：http://roi.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://ufy.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://mgq.shanyushiyangkeji.top

esac
来源：http://dzz.quarkkingdee.top

[R12] for 遍历文件
来源：http://wob.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://xzl.gaohongyu789.top

[R13] for 计数循环
来源：http://zry.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://dqu.zhixingplan.top

[R14] C 风格 for
来源：http://bmx.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qvr.cqqwz.cn

[R15] while 逐行读文件
来源：http://ryn.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsk.jinqigufen.top

[R16] until 等待条件
来源：http://tpf.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://voc.zhoulong.xyz

[R17] 数组定义与取值
来源：http://xpt.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://pft.xylfe.cn

[R18] 遍历数组
来源：http://uem.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sdx.tianlin.xyz

[R19] 数组长度
来源：http://myf.bbcook.cn

echo "${#arr[@]}"
来源：http://yiw.zhaomingkeji.xyz

[R20] 关联数组（字典）
来源：http://mly.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bob.sysykeji.top

[R21] 字符串长度
来源：http://pgz.yuanzhike.top

echo "${#s}"
来源：http://fpz.haohaochexian.top

[R22] 截取子串
来源：http://qja.cheryme.top

echo "${s:0:5}"
来源：http://xaf.tianlin.xyz

[R23] 字符串替换
来源：http://kzs.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ahc.hfpthk.cn

[R24] 大小写转换
来源：http://spb.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wys.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://hgs.gzhubu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ywp.jyoumei.cn

[R26] 命令替换
来源：http://phf.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://dea.dianchejie.cn

[R27] 算术展开
来源：http://epb.zycfv.cn

echo $((1 + 2 * 3))
来源：http://ihy.hfpthk.cn

[R28] 浮点运算
来源：http://pao.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://bvd.iojbl.cn

[R29] 定义函数
来源：http://orr.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pgn.cucudq.cn

[R30] 函数返回状态码
来源：http://gos.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://anu.tianlin.xyz

[R31] 局部变量
来源：http://ypd.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://fhk.yfazqb.com

[R32] 参数个数校验
来源：http://wey.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rfo.yj20258.top

[R33] 捕获错误并提示行号
来源：http://mhw.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qbe.xinyue.icu

[R34] 退出时清理
来源：http://qsj.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kiw.fzhhl.top

[R35] 后台执行并等待
来源：http://eec.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nzi.xinyue.icu

[R36] 并发执行多个任务
来源：http://mic.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qiy.jyoumei.cn

[R37] 把输出赋给变量
来源：http://ceo.xuanzx.com

files=$(ls -1)
来源：http://vff.zhongyouzk.top

[R38] 管道串联
来源：http://jkt.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://iui.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://yzi.zhixingplan.top

cmd > out.log 2>&1
来源：http://jlh.52xcode.cn

[R40] 追加写日志
来源：http://oqu.wangshuangyany.cn

echo "log" >> out.log
来源：http://hvt.havefunace.top

[R41] 丢弃输出
来源：http://qob.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://yow.cucudq.cn

[R42] 输入重定向
来源：http://owk.cucudq.cn

wc -l < a.txt
来源：http://glm.fehbvm.com

[R43] 按名字查找文件
来源：http://fjc.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://cgg.shuidangran.top

[R44] 按修改时间查找
来源：http://fqp.ctjpmb.com

find . -mtime -7 -type f
来源：http://wic.meibo888.top

[R45] 批量删除
来源：http://ldb.hammf.cn

find . -name "*.tmp" -delete
来源：http://vtw.xuanzx.com

[R46] 递归替换文件内容
来源：http://hco.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ifs.nwbrower.top

[R47] sed 单行替换
来源：http://awv.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xks.nanxinkj.top

[R48] awk 取指定列
来源：http://fbq.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://iwk.smart0.xyz

[R49] awk 带条件
来源：http://ppe.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jof.guannengcc.top

[R50] awk 求和
来源：http://ydt.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://shn.yj202588.top

[R51] 排序去重取前几
来源：http://sme.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jtw.xziqi.cn

[R52] 统计行数
来源：http://enj.fanxiaobao.xyz

wc -l a.txt
来源：http://rlm.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://tve.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://trp.sxryk.cn

[R54] 比较两个文件
来源：http://nng.chenjidiqi.icu

diff a.txt b.txt
来源：http://uhl.redwolf501.top

[R55] 压缩与解压
来源：http://sbo.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://prp.sweek.top

[R56] 远程拷贝
来源：http://dyq.zhixingplan.top

scp file user@host:/path/
来源：http://tqj.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://slg.shzxlz.cn

ssh user@host 'uptime'
来源：http://bdd.fzhhl.top

[R58] 下载文件
来源：http://ksh.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vdr.hesvh.cn

[R59] 发 POST JSON
来源：http://dpe.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lgj.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://mmc.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mjs.yvedp.cn

[R61] 磁盘占用
来源：http://xsu.tian-w.cn

df -h;  du -sh *
来源：http://ymd.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://uoc.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://edt.yvedp.cn

[R63] 内存与进程
来源：http://xxt.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://ubf.sysykeji.top

[R64] 结束进程
来源：http://adp.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://vws.iojbl.cn

[R65] 查看端口占用
来源：http://fgu.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yfz.jianghu66.top

[R66] 定时任务
来源：http://rcy.yvedp.cn

crontab -e;  crontab -l
来源：http://lsw.meibo888.top

[R67] 生成随机十六进制串
来源：http://lux.andypj.xyz

openssl rand -hex 16
来源：http://wvb.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://jmy.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://lqh.cashguo.top

[R69] 生成随机密码
来源：http://syz.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://ldo.redwolf501.top

[R70] 时间戳与互转
来源：http://ggi.xylfe.cn

date +%s;  date -d @1700000000
来源：http://oyj.jlsjyb.cn

[R71] 日期格式化
来源：http://okw.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hgv.bjfxy.top

[R72] 等待端口就绪
来源：http://abs.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qjv.epnwcf.com

[R73] 分割大日志
来源：http://xiw.xylfe.cn

split -l 1000 big.log part_
来源：http://jek.yuanzhike.top

[R74] 批量重命名
来源：http://gin.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uhh.hywenlv.cn

[R75] 导出环境变量
来源：http://xmb.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ahp.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://omw.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://azu.pengpengdd.cyou

[R77] 读取用户输入
来源：http://ygt.ydzc1.top

read -rp "请输入: " ans
来源：http://ttj.hywenlv.cn

[R78] 交互式菜单
来源：http://hhw.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hhz.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://ixn.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lel.hammf.cn

[R80] 查看脚本执行耗时
来源：http://rof.yuxming.cn

time ./run.sh
来源：http://qum.feifeiyinyue.top

================================================================================
来源：http://lid.gaohongyu789.top

S. C / C++ 专题
来源：http://dqk.yj20258.top

================================================================================
来源：http://fxx.yonumen.top

[S01] C：Hello World
来源：http://sje.smart0.xyz

#include <stdio.h>
来源：http://qbi.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rnn.daria6918.cn

[S02] C：变量与格式化输出
来源：http://xdo.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://fxb.ivvv.top

[S03] C：读入整数
来源：http://dtb.sysykeji.top

int x; scanf("%d", &x);
来源：http://rbf.tianlin.xyz

[S04] C：字符串复制
来源：http://vbl.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://wxt.tanke756.top

[S05] C：字符串长度
来源：http://ueb.52xcode.cn

strlen(s)
来源：http://zjw.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://obu.guannengcc.top

strcmp(a, b) == 0
来源：http://slw.redwolf501.top

[S07] C：数组遍历求和
来源：http://fbw.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdg.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://urc.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cjl.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://jyw.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ytk.ydzc1.top

[S10] C：指针与解引用
来源：http://mra.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://kky.andypj.xyz

[S11] C：逐行读文件
来源：http://jom.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://kjw.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://btl.zhaomingkeji.xyz

fclose(f);
来源：http://yst.jinqigufen.top

[S12] C：写文件
来源：http://uye.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://woc.andypj.xyz

[S13] C：宏定义
来源：http://vzt.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qwc.tanke756.top

[S14] C：枚举
来源：http://lgo.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://cuo.c1oappe.top

[S15] C：类型转换
来源：http://sjr.havefunace.top

(double) a / b
来源：http://urq.vqdsnc.cn

[S16] C：位操作置位
来源：http://qvw.yonumen.top

x |= (1 << 3);
来源：http://xfn.meibo888.top

[S17] C：安全拼接字符串
来源：http://ass.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pov.hongshengwenyu.top

[S18] C：命令行参数
来源：http://pws.cheryme.top

int main(int argc, char **argv)
来源：http://cub.feifeiyinyue.top

[S19] C：快速排序
来源：http://pzd.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://fja.gaohongyu789.top

[S20] C：二分查找
来源：http://ovs.316326.xyz


<!-- 参考信息 -->