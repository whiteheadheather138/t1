代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kwz.wangdashe.top

[Q58] 累计求和
来源：http://kea.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rrl.jyoumei.cn

[Q59] 分组内累计
来源：http://udd.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bqi.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://blm.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ngz.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://exi.birdmap.top

[Q61] 移动平均
来源：http://jfn.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gum.cashguo.top

[Q62] 分组占比
来源：http://uer.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bps.dashuyun.cn

[Q63] 开启事务
来源：http://myu.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cel.cashguo.top

[Q64] 提交事务
来源：http://lrq.sufxvd.cn

COMMIT;
来源：http://fgc.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://oph.tanke756.top

ROLLBACK;
来源：http://ikt.jinqigfzy.top

[Q66] 行锁查询
来源：http://fqe.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://djl.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://xuz.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ywt.shzxlz.cn

[Q68] 保存点
来源：http://iws.jinqigufen.top

SAVEPOINT sp1;
来源：http://msf.ctjpmb.com

ROLLBACK TO sp1;
来源：http://oqq.hnqzz.top

[Q69] 查看执行计划
来源：http://xjw.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://anv.cqqwz.cn

[Q70] 更新统计信息
来源：http://auz.9152youxi.cn

ANALYZE TABLE users;
来源：http://trt.redwolf501.top

[Q71] 查看建表语句
来源：http://ebz.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tvr.zhiwuduotai.top

[Q72] 查看索引
来源：http://rpb.xinyue.icu

SHOW INDEX FROM users;
来源：http://zhx.hysaishi.cn

[Q73] 查看表状态
来源：http://ona.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qyh.xziqi.cn

[Q74] 强制使用索引
来源：http://pwo.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://apf.hnqzz.top

[Q75] 日期格式化
来源：http://fwg.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kcb.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uzr.hcnkem.com

[Q76] 按天统计
来源：http://jtd.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fdv.daria6918.cn

[Q77] 时间加减
来源：http://cpf.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dwz.iojbl.cn

[Q78] 当前时间
来源：http://ypf.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tdx.yj20258.top

[Q79] 字符串拼接
来源：http://mrd.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://adt.yangfankeji.com

[Q80] 字符串截取
来源：http://iti.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wza.sjlbkw.cn

[Q81] 字符串替换
来源：http://gxj.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aet.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://dld.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cos.jianghu66.top

[Q83] 大小写转换
来源：http://blf.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mcc.daxiang520.top

[Q84] 去除首尾空格
来源：http://nlc.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://xof.yanxiufei.cn

[Q85] 数值取整
来源：http://soy.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wom.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://mha.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xqx.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://njv.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lxv.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://bnk.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fbn.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://etj.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://ykd.chenjidiqi.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tkp.nwbrower.top

[Q90] 生成序号列
来源：http://lcp.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jry.9152youxi.cn

================================================================================
来源：http://urq.iojbl.cn

R. Bash 专题
来源：http://jgs.zhoulong.xyz

================================================================================
来源：http://klh.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://bbt.epnwcf.com

#!/usr/bin/env bash
来源：http://sxz.pengpengdd.cyou

set -euo pipefail
来源：http://zmb.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://ozn.cdnleiting.top

name="Tom"; echo "$name"
来源：http://hcv.svipenyu.cn

[R03] 只读变量
来源：http://bkh.svipenyu.cn

readonly PI=3.14
来源：http://dih.jinghuilouyu.cn

[R04] 位置参数
来源：http://qlf.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zkv.zhiwuduotai.top

[R05] 参数默认值
来源：http://qfq.gotoacloud.top

name="${1:-default}"
来源：http://mwh.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://itg.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kps.sjlbkw.cn

[R07] if 判断文件
来源：http://juz.tarul.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krp.pengpengdd.cyou

[R08] 数值比较
来源：http://bhv.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hcm.cucudq.cn

[R09] 字符串比较
来源：http://okl.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ybv.nanxinkj.top

[R10] 正则匹配
来源：http://rua.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xde.jiagoushi.top

[R11] case 多分支
来源：http://mon.zhaomingkeji.xyz

case "$1" in
来源：http://wjv.pengpengdd.cyou

start) echo "启动" ;;
来源：http://uzm.ydzc1.top

stop)  echo "停止" ;;
来源：http://efx.daria6918.cn

*)     echo "未知命令" ;;
来源：http://gps.haohaochexian.top

esac
来源：http://nit.sufxvd.cn

[R12] for 遍历文件
来源：http://hqq.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://mgj.hcnkem.com

[R13] for 计数循环
来源：http://xva.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://dzq.xuetiantiany.cn

[R14] C 风格 for
来源：http://kdf.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ikf.sufxvd.cn

[R15] while 逐行读文件
来源：http://nry.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rex.gogol.net.cn

[R16] until 等待条件
来源：http://mig.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://osw.xuanzx.com

[R17] 数组定义与取值
来源：http://gic.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ebt.ppjwa.cn

[R18] 遍历数组
来源：http://djc.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vsr.tarul.cn

[R19] 数组长度
来源：http://qkh.mhx1999.top

echo "${#arr[@]}"
来源：http://jqp.tarul.cn

[R20] 关联数组（字典）
来源：http://hlm.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://svm.gogol.net.cn

[R21] 字符串长度
来源：http://hrm.fzhhl.top

echo "${#s}"
来源：http://tps.uphjek.com

[R22] 截取子串
来源：http://rgq.yanxiufei.cn

echo "${s:0:5}"
来源：http://bnx.shuidangran.top

[R23] 字符串替换
来源：http://kuu.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eon.cucudq.cn

[R24] 大小写转换
来源：http://xhk.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://lvb.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://mey.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lbo.fehbvm.com

[R26] 命令替换
来源：http://emj.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://cgq.wangshuangyany.cn

[R27] 算术展开
来源：http://way.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://gte.tarul.cn

[R28] 浮点运算
来源：http://nwo.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://jzq.daxiang520.top

[R29] 定义函数
来源：http://dga.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://shs.zycfv.cn

[R30] 函数返回状态码
来源：http://gmk.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://qdv.daria6918.cn

[R31] 局部变量
来源：http://rpc.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://mbx.sufxvd.cn

[R32] 参数个数校验
来源：http://fct.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qld.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://zxc.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eha.aizwys.cn

[R34] 退出时清理
来源：http://eyz.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://vzm.hammf.cn

[R35] 后台执行并等待
来源：http://ewn.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zek.xinyue.icu

[R36] 并发执行多个任务
来源：http://olm.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tte.ybcxt.top

[R37] 把输出赋给变量
来源：http://wcj.cucudq.cn

files=$(ls -1)
来源：http://iqp.shanyushiyangtech.top

[R38] 管道串联
来源：http://hih.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://cll.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://qde.yfazqb.com

cmd > out.log 2>&1
来源：http://twp.c1oappe.top

[R40] 追加写日志
来源：http://uod.pengpengdd.cyou

echo "log" >> out.log
来源：http://syh.uphjek.com

[R41] 丢弃输出
来源：http://thq.hesvh.cn

cmd >/dev/null 2>&1
来源：http://cls.bbcook.cn

[R42] 输入重定向
来源：http://yuj.quarkkingdee.top

wc -l < a.txt
来源：http://rks.pycfn.com

[R43] 按名字查找文件
来源：http://ber.yueranfly.top

find . -name "*.log" -type f
来源：http://khg.hywenlv.cn

[R44] 按修改时间查找
来源：http://hem.tianlin.xyz

find . -mtime -7 -type f
来源：http://ise.fehbvm.com

[R45] 批量删除
来源：http://kju.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://rkk.cashguo.top

[R46] 递归替换文件内容
来源：http://vli.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nra.mhx1999.top

[R47] sed 单行替换
来源：http://pej.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://hlv.hnxiangtu.top

[R48] awk 取指定列
来源：http://ydb.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://kto.meibo888.top

[R49] awk 带条件
来源：http://txt.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mre.zhixingplan.top

[R50] awk 求和
来源：http://ffb.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://blv.gogol.net.cn

[R51] 排序去重取前几
来源：http://cdj.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xio.dianchejie.cn

[R52] 统计行数
来源：http://lhd.zhixingplan.top

wc -l a.txt
来源：http://pmj.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://ibr.yj20258888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dei.aizwys.cn

[R54] 比较两个文件
来源：http://pwj.hesvh.cn

diff a.txt b.txt
来源：http://blz.ehwqpu.com

[R55] 压缩与解压
来源：http://xej.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dlu.aibaodan.cn

[R56] 远程拷贝
来源：http://sfm.zycfv.cn

scp file user@host:/path/
来源：http://iby.cucudq.cn

[R57] 远程执行命令
来源：http://mks.sufxvd.cn

ssh user@host 'uptime'
来源：http://ogz.hesvh.cn

[R58] 下载文件
来源：http://kqo.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qqg.quarkkingdee.top

[R59] 发 POST JSON
来源：http://nhi.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qaw.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://oms.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jzh.guowangkeji.top

[R61] 磁盘占用
来源：http://psp.kuanghao11.cn

df -h;  du -sh *
来源：http://rom.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://hcd.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://edw.epnwcf.com

[R63] 内存与进程
来源：http://emy.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://bgc.chenlongwang.top

[R64] 结束进程
来源：http://hlw.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://nbq.nanxinkj.top

[R65] 查看端口占用
来源：http://oyp.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytc.zhengqikj.top

[R66] 定时任务
来源：http://ldh.zdbjq.cn

crontab -e;  crontab -l
来源：http://kfw.tarul.cn

[R67] 生成随机十六进制串
来源：http://wzl.hfpthk.cn

openssl rand -hex 16
来源：http://kog.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://azp.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://cxm.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://sqg.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://rgv.gogol.net.cn

[R70] 时间戳与互转
来源：http://wbj.yj20258888.top

date +%s;  date -d @1700000000
来源：http://zgl.zhijiandao.cn

[R71] 日期格式化
来源：http://pka.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwn.0kj1m.cn

[R72] 等待端口就绪
来源：http://xtu.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zor.haohaochexian.top

[R73] 分割大日志
来源：http://pma.hfpthk.cn

split -l 1000 big.log part_
来源：http://mgn.yuxming.cn

[R74] 批量重命名
来源：http://jxi.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://feu.zhixingplan.top

[R75] 导出环境变量
来源：http://gzj.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://aox.jlsjyb.cn

[R76] 使用临时文件
来源：http://gtn.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rrs.jqgfzy.top

[R77] 读取用户输入
来源：http://wvh.havefunace.top

read -rp "请输入: " ans
来源：http://egl.jqgfzy.top

[R78] 交互式菜单
来源：http://kzd.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lrb.zhijiandao.cn

[R79] 解析命令行选项
来源：http://vfx.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hqy.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://ynr.yonumen.top

time ./run.sh
来源：http://fpe.yangfankeji.com

================================================================================
来源：http://ubb.hysaishi.cn

S. C / C++ 专题
来源：http://mpg.hnxiangtu.top

================================================================================
来源：http://myo.sjlbkw.cn

[S01] C：Hello World
来源：http://cmj.zhiwuduotai.top

#include <stdio.h>
来源：http://hoa.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://grz.ivvv.top

[S02] C：变量与格式化输出
来源：http://uev.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://czz.zhoulong.xyz

[S03] C：读入整数
来源：http://yvz.yj20258888.top

int x; scanf("%d", &x);
来源：http://xmr.jinqigufen.top

[S04] C：字符串复制
来源：http://mnj.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://agy.aizwys.cn

[S05] C：字符串长度
来源：http://oac.hongshengwenyu.top

strlen(s)
来源：http://fwi.yfazqb.com

[S06] C：字符串比较
来源：http://jhe.fktsv.cn

strcmp(a, b) == 0
来源：http://zot.sweek.top

[S07] C：数组遍历求和
来源：http://rli.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qvt.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://yio.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://whx.316326.xyz

[S09] C：结构体定义与初始化
来源：http://oop.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xxh.zhijiandao.cn

[S10] C：指针与解引用
来源：http://aaf.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://kid.ydjk.org.cn

[S11] C：逐行读文件
来源：http://vtz.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://lgm.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gdw.sxryk.cn

fclose(f);
来源：http://icq.yuxming.cn

[S12] C：写文件
来源：http://nlt.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dak.zhixingplan.top

[S13] C：宏定义
来源：http://ybj.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrc.ydzc1.top

[S14] C：枚举
来源：http://wuf.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://ibd.mhx1999.top

[S15] C：类型转换
来源：http://bbn.mhx1999.top

(double) a / b
来源：http://ijc.316326.xyz

[S16] C：位操作置位
来源：http://qhp.shangyingyoupin.top

x |= (1 << 3);
来源：http://ixd.yj20258.top

[S17] C：安全拼接字符串
来源：http://zwx.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gwf.zhoulong.xyz

[S18] C：命令行参数
来源：http://frw.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://cnq.yangfankeji.com

[S19] C：快速排序
来源：http://zvk.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eou.ybcxt.top

[S20] C：二分查找
来源：http://shq.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krd.zhixingplan.top

[S21] C：字符类别判断
来源：http://xxq.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://znu.andypj.xyz

[S22] C：字符串转数字
来源：http://wuq.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://suc.nanxuanxn.top

[S23] C：随机数
来源：http://nxw.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ahj.dashuyun.cn

[S24] C：获取本地时间
来源：http://jsn.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://geq.wangdashe.top

[S25] C：内存拷贝
来源：http://zdb.cheryme.top

memcpy(dst, src, n);
来源：http://twi.pycfn.com

[S26] C：内存清零
来源：http://hbq.yueranfly.top

memset(a, 0, sizeof a);
来源：http://ona.wangshuangyany.cn

[S27] C：定义常量
来源：http://lth.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://hwh.sjlbkw.cn

[S28] C：静态变量
来源：http://xbp.tianlin.xyz


<!-- 参考信息 -->