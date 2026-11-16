代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uhw.havefunace.top

[Q52] 删除指定行
来源：http://ocg.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://dlq.zhengqikj.top

[Q53] 按条件删除
来源：http://vng.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sup.daria6918.cn

[Q54] 清空表
来源：http://kqc.bjfxy.top

TRUNCATE TABLE logs;
来源：http://nij.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://ivv.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qll.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://vfq.vehdjk.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hiz.shanyushiyangtech.top

[Q57] 行号
来源：http://cjx.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqv.xuanzx.com

[Q58] 累计求和
来源：http://mzu.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rii.jianghu66.top

[Q59] 分组内累计
来源：http://fpy.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://atd.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://wya.yfazqb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://goc.hnxiangtu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csn.tarul.cn

[Q61] 移动平均
来源：http://yef.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qca.guowangkeji.top

[Q62] 分组占比
来源：http://aqk.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dgn.dashuyun.cn

[Q63] 开启事务
来源：http://itn.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mxn.yanxiufei.cn

[Q64] 提交事务
来源：http://dif.xylfe.cn

COMMIT;
来源：http://wdz.smart0.xyz

[Q65] 回滚事务
来源：http://jfx.gaohongyu789.top

ROLLBACK;
来源：http://trx.zdqjudy.top

[Q66] 行锁查询
来源：http://xhi.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wxn.9152youxi.cn

[Q67] 设置隔离级别
来源：http://prw.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://smp.meibo888.top

[Q68] 保存点
来源：http://myo.fehbvm.com

SAVEPOINT sp1;
来源：http://hxu.yangfankeji.com

ROLLBACK TO sp1;
来源：http://ktb.shzxlz.cn

[Q69] 查看执行计划
来源：http://uxx.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lrm.sjlbkw.cn

[Q70] 更新统计信息
来源：http://pfa.yangfankeji.com

ANALYZE TABLE users;
来源：http://ccw.kuanghao11.cn

[Q71] 查看建表语句
来源：http://sdf.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bqd.zhoulong.xyz

[Q72] 查看索引
来源：http://bpv.zycfv.cn

SHOW INDEX FROM users;
来源：http://eeg.bjfxy.top

[Q73] 查看表状态
来源：http://iwk.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bvm.shzxlz.cn

[Q74] 强制使用索引
来源：http://ser.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hzi.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://ldb.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hdj.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://okz.tanke756.top

[Q76] 按天统计
来源：http://vlf.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oob.mhx1999.top

[Q77] 时间加减
来源：http://smg.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mgj.dianchejie.cn

[Q78] 当前时间
来源：http://kmb.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cca.tianlin.xyz

[Q79] 字符串拼接
来源：http://gkm.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mcj.zhoulong.xyz

[Q80] 字符串截取
来源：http://gqj.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hbu.nwbrower.top

[Q81] 字符串替换
来源：http://zbt.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iac.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://rjs.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vpy.0kj1m.cn

[Q83] 大小写转换
来源：http://cjw.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pwn.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://pjb.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://ysf.hnqzz.top

[Q85] 数值取整
来源：http://cwu.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iuj.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://fxk.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://udr.yueranfly.top

[Q87] JSON 字段做条件
来源：http://bkr.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ovi.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://xif.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bvo.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ges.gzhubu.top

[Q89] 判断表是否存在
来源：http://svu.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vcs.dashuyun.cn

[Q90] 生成序号列
来源：http://bss.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rdc.sweek.top

================================================================================
来源：http://skh.feifeiyinyue.top

R. Bash 专题
来源：http://ioo.hongshengwenyu.top

================================================================================
来源：http://zsx.tian-w.cn

[R01] shebang 与严格模式
来源：http://frn.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://sjl.guannengcc.top

set -euo pipefail
来源：http://tcm.ehwqpu.com

[R02] 变量赋值与使用
来源：http://mri.zhixingplan.top

name="Tom"; echo "$name"
来源：http://vyu.yuxming.cn

[R03] 只读变量
来源：http://gxy.bbcook.cn

readonly PI=3.14
来源：http://ity.shanyushiyangkeji.top

[R04] 位置参数
来源：http://psr.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://slj.uphjek.com

[R05] 参数默认值
来源：http://ebx.uphjek.com

name="${1:-default}"
来源：http://nzx.tian-w.cn

[R06] 判断命令是否存在
来源：http://moo.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dfu.nanxinkj.top

[R07] if 判断文件
来源：http://ytf.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ytd.ehwqpu.com

[R08] 数值比较
来源：http://cuw.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://noo.cheryme.top

[R09] 字符串比较
来源：http://eqv.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hje.andypj.xyz

[R10] 正则匹配
来源：http://etr.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rgy.xuanzx.com

[R11] case 多分支
来源：http://jue.hfpthk.cn

case "$1" in
来源：http://dwa.wangdashe.top

start) echo "启动" ;;
来源：http://ymr.yongpay.top

stop)  echo "停止" ;;
来源：http://nmc.uphjek.com

*)     echo "未知命令" ;;
来源：http://ysr.sjlbkw.cn

esac
来源：http://rrr.havefunace.top

[R12] for 遍历文件
来源：http://aqo.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://hwv.yj202588.top

[R13] for 计数循环
来源：http://qer.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://xsz.vqdsnc.cn

[R14] C 风格 for
来源：http://sub.hnqzz.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tfc.ehwqpu.com

[R15] while 逐行读文件
来源：http://jou.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nbm.jinqigufen.top

[R16] until 等待条件
来源：http://wsv.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ohz.guowangkeji.top

[R17] 数组定义与取值
来源：http://yrq.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xrn.chenjidiqi.icu

[R18] 遍历数组
来源：http://nvn.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nxt.daxiang520.top

[R19] 数组长度
来源：http://efb.hnqzz.top

echo "${#arr[@]}"
来源：http://gtz.cheryme.top

[R20] 关联数组（字典）
来源：http://nde.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sgn.wangdashe.top

[R21] 字符串长度
来源：http://ojq.jinqigufen.top

echo "${#s}"
来源：http://hxa.nwbrower.top

[R22] 截取子串
来源：http://frp.yanxiufei.cn

echo "${s:0:5}"
来源：http://lgm.pycfn.com

[R23] 字符串替换
来源：http://vdi.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nua.zhengqikj.top

[R24] 大小写转换
来源：http://saz.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jqo.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://ckc.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rnw.fengsongda.top

[R26] 命令替换
来源：http://eug.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://hjm.hywenlv.cn

[R27] 算术展开
来源：http://rbq.mhx1999.top

echo $((1 + 2 * 3))
来源：http://ykp.fengsongda.top

[R28] 浮点运算
来源：http://uvx.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://mqg.yueranfly.top

[R29] 定义函数
来源：http://tkq.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cqt.ydjk.org.cn

[R30] 函数返回状态码
来源：http://sav.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://ady.ybcxt.top

[R31] 局部变量
来源：http://wmu.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://gvb.zhijiandao.cn

[R32] 参数个数校验
来源：http://xbh.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wul.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://plm.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lur.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://quh.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://say.nwbrower.top

[R35] 后台执行并等待
来源：http://orf.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ogw.9152youxi.cn

[R36] 并发执行多个任务
来源：http://ebu.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exp.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://zts.chenzaomai.com

files=$(ls -1)
来源：http://mzt.nwbrower.top

[R38] 管道串联
来源：http://uwn.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://mzk.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://ttc.fzhhl.top

cmd > out.log 2>&1
来源：http://tmn.yuanzhike.top

[R40] 追加写日志
来源：http://bsd.daxiang520.top

echo "log" >> out.log
来源：http://bog.wangdashe.top

[R41] 丢弃输出
来源：http://qnh.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://cyo.hnqzz.top

[R42] 输入重定向
来源：http://cqb.tanke756.top

wc -l < a.txt
来源：http://sok.hcnkem.com

[R43] 按名字查找文件
来源：http://hki.meibo888.top

find . -name "*.log" -type f
来源：http://kzi.dashuyun.cn

[R44] 按修改时间查找
来源：http://wjr.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://ryh.sxryk.cn

[R45] 批量删除
来源：http://uhh.daria6918.cn

find . -name "*.tmp" -delete
来源：http://npj.c1oappe.top

[R46] 递归替换文件内容
来源：http://mmo.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://suv.ivvv.top

[R47] sed 单行替换
来源：http://cci.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://lrj.tarul.cn

[R48] awk 取指定列
来源：http://hsl.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://geo.sysykeji.top

[R49] awk 带条件
来源：http://ebq.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yoa.jianghu66.top

[R50] awk 求和
来源：http://lfy.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://sdh.redwolf501.top

[R51] 排序去重取前几
来源：http://rxm.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pyu.c1oappe.top

[R52] 统计行数
来源：http://zgh.wangshuangyany.cn

wc -l a.txt
来源：http://ypa.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://bzb.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://opo.hammf.cn

[R54] 比较两个文件
来源：http://lrk.fzhhl.top

diff a.txt b.txt
来源：http://sni.zycfv.cn

[R55] 压缩与解压
来源：http://ksw.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gzm.tianlin.xyz

[R56] 远程拷贝
来源：http://baq.bbcook.cn

scp file user@host:/path/
来源：http://woo.mhx1999.top

[R57] 远程执行命令
来源：http://mjp.andypj.xyz

ssh user@host 'uptime'
来源：http://sus.shanyushiyangtech.top

[R58] 下载文件
来源：http://lfu.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ckh.xziqi.cn

[R59] 发 POST JSON
来源：http://jfy.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://brg.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://fhc.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rxg.redwolf501.top

[R61] 磁盘占用
来源：http://cks.cdnleiting.top

df -h;  du -sh *
来源：http://iyp.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://hdq.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://hba.chenzaomai.com

[R63] 内存与进程
来源：http://fxj.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://flj.hfpthk.cn

[R64] 结束进程
来源：http://kxs.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://emv.iojbl.cn

[R65] 查看端口占用
来源：http://rfr.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zdb.tanke756.top

[R66] 定时任务
来源：http://abu.gaohongyu789.top

crontab -e;  crontab -l
来源：http://yik.yuxming.cn

[R67] 生成随机十六进制串
来源：http://tip.dianchejie.cn

openssl rand -hex 16
来源：http://hjk.jinqigfzy.top

[R68] 计算文件校验值
来源：http://auw.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://oar.sjlbkw.cn

[R69] 生成随机密码
来源：http://hje.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://wyi.0kj1m.cn

[R70] 时间戳与互转
来源：http://acx.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://bln.316326.xyz

[R71] 日期格式化
来源：http://qzt.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://owj.sxryk.cn

[R72] 等待端口就绪
来源：http://wqo.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://plt.ivvv.top

[R73] 分割大日志
来源：http://vav.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://yhm.jinqigufen.top

[R74] 批量重命名
来源：http://otg.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gie.gogol.net.cn

[R75] 导出环境变量
来源：http://bde.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://zky.xinyue.icu

[R76] 使用临时文件
来源：http://suy.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://enz.mhx1999.top

[R77] 读取用户输入
来源：http://awu.ctjpmb.com

read -rp "请输入: " ans
来源：http://ixv.cheryme.top

[R78] 交互式菜单
来源：http://ydo.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pcp.andypj.xyz

[R79] 解析命令行选项
来源：http://dav.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qov.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://zyt.vehdjk.com

time ./run.sh
来源：http://peb.sufxvd.cn

================================================================================
来源：http://nwq.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://ivd.yangfankeji.com

================================================================================
来源：http://isf.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://pcn.snrcjt.cn

#include <stdio.h>
来源：http://czn.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nnj.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://ywl.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://ajy.xuetiantiany.cn

[S03] C：读入整数
来源：http://zhr.iojbl.cn

int x; scanf("%d", &x);
来源：http://iqj.52xcode.cn

[S04] C：字符串复制
来源：http://xcj.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://dgp.zhengqikj.top

[S05] C：字符串长度
来源：http://liu.hcnkem.com

strlen(s)
来源：http://tzw.fktsv.cn

[S06] C：字符串比较
来源：http://wvo.hywenlv.cn

strcmp(a, b) == 0
来源：http://lij.jyoumei.cn

[S07] C：数组遍历求和
来源：http://qak.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rss.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://ruu.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aus.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://vaa.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hoa.yueranfly.top

[S10] C：指针与解引用
来源：http://tky.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://wkp.aibaodan.cn

[S11] C：逐行读文件
来源：http://vmn.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://uep.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iex.hongshengwenyu.top

fclose(f);
来源：http://npy.quarkkingdee.top

[S12] C：写文件
来源：http://lwv.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gzy.guowangkeji.top

[S13] C：宏定义
来源：http://fam.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cup.jqgufenzy.top

[S14] C：枚举
来源：http://lfs.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://bkb.hesvh.cn

[S15] C：类型转换
来源：http://xsa.yonumen.top

(double) a / b
来源：http://iod.jqgfzy.top

[S16] C：位操作置位
来源：http://mpn.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://kct.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://apn.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bdw.snrcjt.cn

[S18] C：命令行参数
来源：http://wov.xinyue.icu

int main(int argc, char **argv)
来源：http://may.smart0.xyz

[S19] C：快速排序
来源：http://lvk.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://bhq.jqgfzy.top

[S20] C：二分查找
来源：http://rgo.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bsx.jinqigfzy.top

[S21] C：字符类别判断
来源：http://val.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cas.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://lrl.tianlin.xyz


<!-- 参考信息 -->