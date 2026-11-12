代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://twt.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://pwv.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yls.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ynx.ppjwa.cn

[Q61] 移动平均
来源：http://ipg.hysaishi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qaj.xuanzx.com

[Q62] 分组占比
来源：http://cbo.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bwo.nanxinkj.top

[Q63] 开启事务
来源：http://jox.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jbu.zdqjudy.top

[Q64] 提交事务
来源：http://mdk.jqgfzy.top

COMMIT;
来源：http://btk.tian-w.cn

[Q65] 回滚事务
来源：http://osv.redwolf501.top

ROLLBACK;
来源：http://oux.cdnleiting.top

[Q66] 行锁查询
来源：http://vke.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tow.ehwqpu.com

[Q67] 设置隔离级别
来源：http://aaz.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsg.tian-w.cn

[Q68] 保存点
来源：http://zjo.yangfankeji.com

SAVEPOINT sp1;
来源：http://zcx.hfpthk.cn

ROLLBACK TO sp1;
来源：http://okh.guannengcc.top

[Q69] 查看执行计划
来源：http://qes.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wgq.jianghu66.top

[Q70] 更新统计信息
来源：http://hgb.zdqjudy.top

ANALYZE TABLE users;
来源：http://mbp.jqgufenzy.top

[Q71] 查看建表语句
来源：http://wvq.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zju.jyoumei.cn

[Q72] 查看索引
来源：http://uwv.gogol.net.cn

SHOW INDEX FROM users;
来源：http://jab.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://icm.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jxp.bjfxy.top

[Q74] 强制使用索引
来源：http://glt.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bhc.hammf.cn

[Q75] 日期格式化
来源：http://isb.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dsm.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blc.haohaochexian.top

[Q76] 按天统计
来源：http://cgo.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eik.hysaishi.cn

[Q77] 时间加减
来源：http://ggc.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://srg.xziqi.cn

[Q78] 当前时间
来源：http://lhr.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wmn.birdmap.top

[Q79] 字符串拼接
来源：http://mcp.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hxi.aizwys.cn

[Q80] 字符串截取
来源：http://sem.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mvh.svipenyu.cn

[Q81] 字符串替换
来源：http://chi.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kzg.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://mhf.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://muh.gotoacloud.top

[Q83] 大小写转换
来源：http://xyr.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oqs.daria6918.cn

[Q84] 去除首尾空格
来源：http://xel.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://gsa.xuanzx.com

[Q85] 数值取整
来源：http://lnl.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://chw.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://rnc.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgn.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://plb.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyl.sweek.top

[Q88] 行转列（条件聚合）
来源：http://atr.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fzo.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://coj.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://npg.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lep.zhixingplan.top

[Q90] 生成序号列
来源：http://nxf.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://azh.shanyushiyangtech.top

================================================================================
来源：http://btr.jianghu66.top

R. Bash 专题
来源：http://zpd.yueranfly.top

================================================================================
来源：http://zdk.jinqigfzy.top

[R01] shebang 与严格模式
来源：http://phe.jqgfzy.top

#!/usr/bin/env bash
来源：http://qhq.gzhubu.top

set -euo pipefail
来源：http://kqn.ydzc1.top

[R02] 变量赋值与使用
来源：http://gbt.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://kzg.shangyingyoupin.top

[R03] 只读变量
来源：http://lza.yvedp.cn

readonly PI=3.14
来源：http://dym.yonumen.top

[R04] 位置参数
来源：http://sgi.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kvl.aizwys.cn

[R05] 参数默认值
来源：http://rzj.ydjk.org.cn

name="${1:-default}"
来源：http://xut.chenzaomai.com

[R06] 判断命令是否存在
来源：http://zkz.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khl.ydzc1.top

[R07] if 判断文件
来源：http://wfs.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tnv.wangdashe.top

[R08] 数值比较
来源：http://kfq.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cmy.xziqi.cn

[R09] 字符串比较
来源：http://ksc.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gjw.aibaodan.cn

[R10] 正则匹配
来源：http://gox.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kys.hnxiangtu.top

[R11] case 多分支
来源：http://nej.yfazqb.com

case "$1" in
来源：http://jni.ivvv.top

start) echo "启动" ;;
来源：http://zrm.xylfe.cn

stop)  echo "停止" ;;
来源：http://xju.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://ans.shuidangran.top

esac
来源：http://ydx.tanke756.top

[R12] for 遍历文件
来源：http://enz.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://kiv.bbcook.cn

[R13] for 计数循环
来源：http://xoq.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://gwu.redwolf501.top

[R14] C 风格 for
来源：http://zyg.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dwx.yuanzhike.top

[R15] while 逐行读文件
来源：http://jzr.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://imo.ctjpmb.com

[R16] until 等待条件
来源：http://vkp.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ifh.sysykeji.top

[R17] 数组定义与取值
来源：http://ygh.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://qhv.cashguo.top

[R18] 遍历数组
来源：http://zky.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qwu.tanke756.top

[R19] 数组长度
来源：http://htu.cqqwz.cn

echo "${#arr[@]}"
来源：http://qbj.sxryk.cn

[R20] 关联数组（字典）
来源：http://ghf.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ivl.wangdashe.top

[R21] 字符串长度
来源：http://ohu.cheryme.top

echo "${#s}"
来源：http://nip.sjlbkw.cn

[R22] 截取子串
来源：http://itb.cheryme.top

echo "${s:0:5}"
来源：http://gox.guannengcc.top

[R23] 字符串替换
来源：http://nbq.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ago.hnqzz.top

[R24] 大小写转换
来源：http://qti.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ena.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://ggv.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cye.dashuyun.cn

[R26] 命令替换
来源：http://kkz.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://qpx.shzxlz.cn

[R27] 算术展开
来源：http://dza.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://jbo.yongpay.top

[R28] 浮点运算
来源：http://vtc.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://tzn.hcnkem.com

[R29] 定义函数
来源：http://ejx.xuetiantiany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vvf.daxiang520.top

[R30] 函数返回状态码
来源：http://sai.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://knd.xuanzx.com

[R31] 局部变量
来源：http://gjj.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://xgz.ydzc1.top

[R32] 参数个数校验
来源：http://pcw.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vqs.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://izm.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://krh.quarkkingdee.top

[R34] 退出时清理
来源：http://nju.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jzp.sxryk.cn

[R35] 后台执行并等待
来源：http://ivi.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://qor.pycfn.com

[R36] 并发执行多个任务
来源：http://hzx.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lso.shzxlz.cn

[R37] 把输出赋给变量
来源：http://xob.tianlin.xyz

files=$(ls -1)
来源：http://bui.hnxiangtu.top

[R38] 管道串联
来源：http://nlu.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://yau.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://zsx.mhx1999.top

cmd > out.log 2>&1
来源：http://pgh.smart0.xyz

[R40] 追加写日志
来源：http://rtd.chenjidiqi.icu

echo "log" >> out.log
来源：http://zdr.hywenlv.cn

[R41] 丢弃输出
来源：http://axt.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://zmz.sweek.top

[R42] 输入重定向
来源：http://cnp.yfazqb.com

wc -l < a.txt
来源：http://pxc.haohaochexian.top

[R43] 按名字查找文件
来源：http://tvc.zdbjq.cn

find . -name "*.log" -type f
来源：http://acz.yj20258.top

[R44] 按修改时间查找
来源：http://gse.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://gzo.hysaishi.cn

[R45] 批量删除
来源：http://vex.aizwys.cn

find . -name "*.tmp" -delete
来源：http://vaw.smart0.xyz

[R46] 递归替换文件内容
来源：http://mwj.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ujn.andypj.xyz

[R47] sed 单行替换
来源：http://xmy.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://jzr.bbcook.cn

[R48] awk 取指定列
来源：http://gym.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://tto.ctjpmb.com

[R49] awk 带条件
来源：http://qgi.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ywj.chenjidiqi.icu

[R50] awk 求和
来源：http://gwh.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fbl.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://pbq.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://obw.ybcxt.top

[R52] 统计行数
来源：http://hdj.zhixingplan.top

wc -l a.txt
来源：http://ykj.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://rte.zdqjudy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sia.52xcode.cn

[R54] 比较两个文件
来源：http://iez.xylfe.cn

diff a.txt b.txt
来源：http://qjd.cdnleiting.top

[R55] 压缩与解压
来源：http://knl.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iui.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://eog.cqqwz.cn

scp file user@host:/path/
来源：http://hdk.yonumen.top

[R57] 远程执行命令
来源：http://ckz.c1oappe.top

ssh user@host 'uptime'
来源：http://coq.shanyushiyangkeji.top

[R58] 下载文件
来源：http://jyu.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ymw.fktsv.cn

[R59] 发 POST JSON
来源：http://mjk.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://udc.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://ils.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bra.haohaochexian.top

[R61] 磁盘占用
来源：http://plo.hesvh.cn

df -h;  du -sh *
来源：http://fcg.nanxinkj.top

[R62] 找最占空间的文件
来源：http://axu.sweek.top

du -ah . | sort -rh | head -10
来源：http://duy.smart0.xyz

[R63] 内存与进程
来源：http://jan.yj20258.top

free -h;  ps aux | grep nginx
来源：http://nti.xziqi.cn

[R64] 结束进程
来源：http://pjt.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://cho.0kj1m.cn

[R65] 查看端口占用
来源：http://txb.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://spa.kuanghao11.cn

[R66] 定时任务
来源：http://ggk.jinqigufen.top

crontab -e;  crontab -l
来源：http://fls.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://cdx.jinghuilouyu.cn

openssl rand -hex 16
来源：http://gux.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://aqh.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://qni.svipenyu.cn

[R69] 生成随机密码
来源：http://xwt.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://bte.chenzaomai.com

[R70] 时间戳与互转
来源：http://cej.yvedp.cn

date +%s;  date -d @1700000000
来源：http://ruh.jlsjyb.cn

[R71] 日期格式化
来源：http://mov.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nzu.sufxvd.cn

[R72] 等待端口就绪
来源：http://ozr.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ivv.vehdjk.com

[R73] 分割大日志
来源：http://geq.ivvv.top

split -l 1000 big.log part_
来源：http://osy.yangfankeji.com

[R74] 批量重命名
来源：http://csx.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uee.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://rtq.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://dxw.dashuyun.cn

[R76] 使用临时文件
来源：http://nkj.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bes.redwolf501.top

[R77] 读取用户输入
来源：http://img.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://tin.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://xec.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zjg.hnqzz.top

[R79] 解析命令行选项
来源：http://nxw.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vyk.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://utf.tarul.cn

time ./run.sh
来源：http://elr.hnqzz.top

================================================================================
来源：http://bqh.uphjek.com

S. C / C++ 专题
来源：http://hzz.mhx1999.top

================================================================================
来源：http://skc.zdqjudy.top

[S01] C：Hello World
来源：http://gqr.tarul.cn

#include <stdio.h>
来源：http://ptm.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmw.iojbl.cn

[S02] C：变量与格式化输出
来源：http://vss.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://wwt.sjlbkw.cn

[S03] C：读入整数
来源：http://eus.52xcode.cn

int x; scanf("%d", &x);
来源：http://hyn.shzxlz.cn

[S04] C：字符串复制
来源：http://wva.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://jzs.gzhubu.top

[S05] C：字符串长度
来源：http://ixg.redwolf501.top

strlen(s)
来源：http://rgw.yangfankeji.com

[S06] C：字符串比较
来源：http://ocd.xylfe.cn

strcmp(a, b) == 0
来源：http://ikq.yangfankeji.com

[S07] C：数组遍历求和
来源：http://hea.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yhl.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://eyo.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wve.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://bij.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hgp.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://ybc.meibo888.top

int *p = &a;  *p = 5;
来源：http://olw.yvedp.cn

[S11] C：逐行读文件
来源：http://tnm.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://iho.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://dan.gaohongyu789.top

fclose(f);
来源：http://zlw.wangshuangyany.cn

[S12] C：写文件
来源：http://sws.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fin.sufxvd.cn

[S13] C：宏定义
来源：http://qhx.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fwp.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://rns.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://lue.hysaishi.cn

[S15] C：类型转换
来源：http://yom.guannengcc.top

(double) a / b
来源：http://enl.meibo888.top

[S16] C：位操作置位
来源：http://kbv.yongpay.top

x |= (1 << 3);
来源：http://qgi.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://mfy.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hqz.zdqjudy.top

[S18] C：命令行参数
来源：http://cmf.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://jxw.hfpthk.cn

[S19] C：快速排序
来源：http://sel.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xab.hfpthk.cn

[S20] C：二分查找
来源：http://fwv.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lds.jianghu66.top

[S21] C：字符类别判断
来源：http://ycl.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vmy.cheryme.top

[S22] C：字符串转数字
来源：http://bfn.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://wzm.ctjpmb.com

[S23] C：随机数
来源：http://uhq.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kqh.nwbrower.top

[S24] C：获取本地时间
来源：http://chl.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kzz.hammf.cn

[S25] C：内存拷贝
来源：http://rpz.zhijiandao.cn

memcpy(dst, src, n);
来源：http://ucf.zdbjq.cn

[S26] C：内存清零
来源：http://yaj.52xcode.cn

memset(a, 0, sizeof a);
来源：http://umd.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://eeo.uphjek.com

const double PI = 3.14159;
来源：http://ako.jiagoushi.top

[S28] C：静态变量
来源：http://kfb.chenjidiqi.icu

static int counter = 0;
来源：http://yfm.yvedp.cn

[S29] C：变参函数
来源：http://igt.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://huq.hysaishi.cn

[S30] C：头文件保护
来源：http://dgo.ppjwa.cn


<!-- 参考信息 -->