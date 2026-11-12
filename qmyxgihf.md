代发 wailian999

[Q61] 移动平均
来源：http://iry.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fir.mhx1999.top

[Q62] 分组占比
来源：http://aeg.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ord.gogol.net.cn

[Q63] 开启事务
来源：http://age.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bxw.jinghuilouyu.cn

[Q64] 提交事务
来源：http://pit.gaohongyu789.top

COMMIT;
来源：http://wgu.sjlbkw.cn

[Q65] 回滚事务
来源：http://oqe.cashguo.top

ROLLBACK;
来源：http://tsq.yongpay.top

[Q66] 行锁查询
来源：http://bej.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qhn.aibaodan.cn

[Q67] 设置隔离级别
来源：http://enb.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xww.fengsongda.top

[Q68] 保存点
来源：http://ghj.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://iir.cashguo.top

ROLLBACK TO sp1;
来源：http://mju.c1oappe.top

[Q69] 查看执行计划
来源：http://kla.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pki.yj202588.top

[Q70] 更新统计信息
来源：http://fnb.fktsv.cn

ANALYZE TABLE users;
来源：http://ait.gzhubu.top

[Q71] 查看建表语句
来源：http://htt.zhaomingkeji.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://key.yj202588.top

[Q72] 查看索引
来源：http://aqx.yongpay.top

SHOW INDEX FROM users;
来源：http://icy.ydjk.org.cn

[Q73] 查看表状态
来源：http://plj.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bsa.sysykeji.top

[Q74] 强制使用索引
来源：http://plg.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tqd.jlsjyb.cn

[Q75] 日期格式化
来源：http://tlu.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nrw.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hud.zhengqikj.top

[Q76] 按天统计
来源：http://jfr.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://frr.c1oappe.top

[Q77] 时间加减
来源：http://kxb.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xda.cheryme.top

[Q78] 当前时间
来源：http://uog.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oau.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://loz.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lqe.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://mgo.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdy.nwbrower.top

[Q81] 字符串替换
来源：http://yqm.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://crf.ivvv.top

[Q82] 字符长度与字节长度
来源：http://dkz.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zxk.hfpthk.cn

[Q83] 大小写转换
来源：http://mim.cheryme.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://khy.yongpay.top

[Q84] 去除首尾空格
来源：http://gdz.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://otx.gogol.net.cn

[Q85] 数值取整
来源：http://evi.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jda.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://byh.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bcf.iojbl.cn

[Q87] JSON 字段做条件
来源：http://pri.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://myz.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://yth.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qrn.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qfs.yuxming.cn

[Q89] 判断表是否存在
来源：http://jhb.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zmp.gaohongyu789.top

[Q90] 生成序号列
来源：http://pwi.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hzm.gogol.net.cn

================================================================================
来源：http://bev.wangdashe.top

R. Bash 专题
来源：http://qgt.nanxuanxn.top

================================================================================
来源：http://vvk.ctjpmb.com

[R01] shebang 与严格模式
来源：http://kih.ppjwa.cn

#!/usr/bin/env bash
来源：http://efu.shangyingyoupin.top

set -euo pipefail
来源：http://fvg.chenlongwang.top

[R02] 变量赋值与使用
来源：http://uvh.wangdashe.top

name="Tom"; echo "$name"
来源：http://snc.nwbrower.top

[R03] 只读变量
来源：http://crv.mhx1999.top

readonly PI=3.14
来源：http://rji.jqgfzy.top

[R04] 位置参数
来源：http://lfv.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ape.uphjek.com

[R05] 参数默认值
来源：http://vdg.shanyushiyangkeji.top

name="${1:-default}"
来源：http://xul.zdqjudy.top

[R06] 判断命令是否存在
来源：http://cdg.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ger.0kj1m.cn

[R07] if 判断文件
来源：http://sxn.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tvu.yangfankeji.com

[R08] 数值比较
来源：http://yoq.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ekm.cdnleiting.top

[R09] 字符串比较
来源：http://hic.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ggy.pengpengdd.cyou

[R10] 正则匹配
来源：http://pje.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qkw.jqgufenzy.top

[R11] case 多分支
来源：http://ckk.sweek.top

case "$1" in
来源：http://nfk.aibaodan.cn

start) echo "启动" ;;
来源：http://dlm.aibaodan.cn

stop)  echo "停止" ;;
来源：http://ooy.xziqi.cn

*)     echo "未知命令" ;;
来源：http://yhf.cqqwz.cn

esac
来源：http://una.xylfe.cn

[R12] for 遍历文件
来源：http://evw.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://bnj.redwolf501.top

[R13] for 计数循环
来源：http://mmb.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://app.xinyue.icu

[R14] C 风格 for
来源：http://orb.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yfm.aizwys.cn

[R15] while 逐行读文件
来源：http://pjj.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://buu.hongshengwenyu.top

[R16] until 等待条件
来源：http://vep.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mln.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://hsa.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xvr.fengsongda.top

[R18] 遍历数组
来源：http://fhc.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dtc.yuxming.cn

[R19] 数组长度
来源：http://ale.jiagoushi.top

echo "${#arr[@]}"
来源：http://flk.tian-w.cn

[R20] 关联数组（字典）
来源：http://vzo.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xpy.ydzc1.top

[R21] 字符串长度
来源：http://bqi.chenjidiqi.icu

echo "${#s}"
来源：http://flw.hywenlv.cn

[R22] 截取子串
来源：http://qrr.shzxlz.cn

echo "${s:0:5}"
来源：http://zux.zdbjq.cn

[R23] 字符串替换
来源：http://jpn.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cbq.316326.xyz

[R24] 大小写转换
来源：http://hmr.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://krv.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://jas.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sji.haohaochexian.top

[R26] 命令替换
来源：http://efb.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://xgx.dashuyun.cn

[R27] 算术展开
来源：http://nuh.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://jnc.yueranfly.top

[R28] 浮点运算
来源：http://ouu.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://bky.fzhhl.top

[R29] 定义函数
来源：http://uoy.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://liv.havefunace.top

[R30] 函数返回状态码
来源：http://abs.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://syo.guannengcc.top

[R31] 局部变量
来源：http://lrj.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://yhr.zycfv.cn

[R32] 参数个数校验
来源：http://kvp.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tlo.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://njf.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hww.chenzaomai.com

[R34] 退出时清理
来源：http://cyj.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://mmw.yvedp.cn

[R35] 后台执行并等待
来源：http://pqh.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mhz.yuanzhike.top

[R36] 并发执行多个任务
来源：http://qcd.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pzf.daxiang520.top

[R37] 把输出赋给变量
来源：http://dfi.yj20258.top

files=$(ls -1)
来源：http://iae.havefunace.top

[R38] 管道串联
来源：http://jmd.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://ogi.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://oky.tian-w.cn

cmd > out.log 2>&1
来源：http://cow.hfpthk.cn

[R40] 追加写日志
来源：http://sxl.epnwcf.com

echo "log" >> out.log
来源：http://sxa.wangshuangyany.cn

[R41] 丢弃输出
来源：http://kzc.hnqzz.top

cmd >/dev/null 2>&1
来源：http://knf.feifeiyinyue.top

[R42] 输入重定向
来源：http://jcg.wangdashe.top

wc -l < a.txt
来源：http://zqx.yfazqb.com

[R43] 按名字查找文件
来源：http://ozt.yueranfly.top

find . -name "*.log" -type f
来源：http://iat.jyoumei.cn

[R44] 按修改时间查找
来源：http://akt.zdqjudy.top

find . -mtime -7 -type f
来源：http://fef.jqgfzy.top

[R45] 批量删除
来源：http://rhr.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://vfd.sysykeji.top

[R46] 递归替换文件内容
来源：http://zxj.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hjd.hongshengwenyu.top

[R47] sed 单行替换
来源：http://zfi.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://ubc.shzxlz.cn

[R48] awk 取指定列
来源：http://yow.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://irl.zhiwuduotai.top

[R49] awk 带条件
来源：http://kxi.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yzi.svipenyu.cn

[R50] awk 求和
来源：http://fxk.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://bmc.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://api.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ynr.vehdjk.com

[R52] 统计行数
来源：http://iqv.aizwys.cn

wc -l a.txt
来源：http://awj.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://qtu.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uuy.fktsv.cn

[R54] 比较两个文件
来源：http://eyq.yuanzhike.top

diff a.txt b.txt
来源：http://vzl.chenzaomai.com

[R55] 压缩与解压
来源：http://neo.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mtq.daria6918.cn

[R56] 远程拷贝
来源：http://ulw.zhiwuduotai.top

scp file user@host:/path/
来源：http://dvd.52xcode.cn

[R57] 远程执行命令
来源：http://eqp.yj202588.top

ssh user@host 'uptime'
来源：http://qbh.yangfankeji.com

[R58] 下载文件
来源：http://fvw.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ghf.nwbrower.top

[R59] 发 POST JSON
来源：http://llr.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skt.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://vob.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nex.zhiwuduotai.top

[R61] 磁盘占用
来源：http://yxa.wangshuangyany.cn

df -h;  du -sh *
来源：http://dsq.xylfe.cn

[R62] 找最占空间的文件
来源：http://ojl.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://mlw.jqgufenzy.top

[R63] 内存与进程
来源：http://mfx.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://wjk.pengpengdd.cyou

[R64] 结束进程
来源：http://wny.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://yuz.sjlbkw.cn

[R65] 查看端口占用
来源：http://aqw.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://apm.hcnkem.com

[R66] 定时任务
来源：http://biz.hammf.cn

crontab -e;  crontab -l
来源：http://lph.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://rou.jlsjyb.cn

openssl rand -hex 16
来源：http://gql.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://lvn.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://cug.tian-w.cn

[R69] 生成随机密码
来源：http://ddf.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://tjt.redwolf501.top

[R70] 时间戳与互转
来源：http://sgj.meibo888.top

date +%s;  date -d @1700000000
来源：http://trr.vehdjk.com

[R71] 日期格式化
来源：http://sta.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nob.nanxinkj.top

[R72] 等待端口就绪
来源：http://xbi.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qzp.yangfankeji.com

[R73] 分割大日志
来源：http://hkq.sjlbkw.cn

split -l 1000 big.log part_
来源：http://nij.gaohongyu789.top

[R74] 批量重命名
来源：http://soo.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gst.shzxlz.cn

[R75] 导出环境变量
来源：http://qgo.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://isr.ctjpmb.com

[R76] 使用临时文件
来源：http://cvr.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zaw.jiagoushi.top

[R77] 读取用户输入
来源：http://qte.chenzaomai.com

read -rp "请输入: " ans
来源：http://ljc.epnwcf.com

[R78] 交互式菜单
来源：http://dou.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xsm.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://zxw.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gbc.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://bjb.jqgfzy.top

time ./run.sh
来源：http://tpn.andypj.xyz

================================================================================
来源：http://gsb.birdmap.top

S. C / C++ 专题
来源：http://sbw.xziqi.cn

================================================================================
来源：http://hwt.yj20258.top

[S01] C：Hello World
来源：http://ona.cqqwz.cn

#include <stdio.h>
来源：http://nrb.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rhc.vehdjk.com

[S02] C：变量与格式化输出
来源：http://rde.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://ydd.c1oappe.top

[S03] C：读入整数
来源：http://ajq.nwbrower.top

int x; scanf("%d", &x);
来源：http://jku.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://pfr.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mdi.kuanghao11.cn

[S05] C：字符串长度
来源：http://zqd.shzxlz.cn

strlen(s)
来源：http://cyw.zhengqikj.top

[S06] C：字符串比较
来源：http://dao.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://vkf.andypj.xyz

[S07] C：数组遍历求和
来源：http://duv.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fyn.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://mhe.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://spv.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://hab.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ysv.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://voz.epnwcf.com

int *p = &a;  *p = 5;
来源：http://bou.yongpay.top

[S11] C：逐行读文件
来源：http://lnm.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://kcv.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zgl.havefunace.top

fclose(f);
来源：http://gnr.cucudq.cn

[S12] C：写文件
来源：http://ive.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://erv.jianghu66.top

[S13] C：宏定义
来源：http://ean.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rch.yuanzhike.top

[S14] C：枚举
来源：http://uih.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://for.pengpengdd.cyou

[S15] C：类型转换
来源：http://ywu.sweek.top

(double) a / b
来源：http://nvi.xziqi.cn

[S16] C：位操作置位
来源：http://yfa.tian-w.cn

x |= (1 << 3);
来源：http://wnv.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://dde.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://had.ctjpmb.com

[S18] C：命令行参数
来源：http://jaz.nanxuanxn.top

int main(int argc, char **argv)
来源：http://dcw.c1oappe.top

[S19] C：快速排序
来源：http://eil.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://atf.zdbjq.cn

[S20] C：二分查找
来源：http://jpt.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ybb.xinyue.icu

[S21] C：字符类别判断
来源：http://uow.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://euk.snrcjt.cn

[S22] C：字符串转数字
来源：http://wru.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://laj.shuidangran.top

[S23] C：随机数
来源：http://vip.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://knr.zhongyouzk.top

[S24] C：获取本地时间
来源：http://hdw.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bib.zhongyouzk.top

[S25] C：内存拷贝
来源：http://dhr.haohaochexian.top

memcpy(dst, src, n);
来源：http://lxh.ctjpmb.com

[S26] C：内存清零
来源：http://zla.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://bfj.redwolf501.top

[S27] C：定义常量
来源：http://ezn.aizwys.cn

const double PI = 3.14159;
来源：http://edd.yongpay.top

[S28] C：静态变量
来源：http://uqs.snrcjt.cn

static int counter = 0;
来源：http://hlj.jlsjyb.cn

[S29] C：变参函数
来源：http://ifb.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eac.jianghu66.top

[S30] C：头文件保护
来源：http://jvj.zhaomingkeji.xyz

#ifndef X_H
来源：http://lae.svipenyu.cn

#define X_H
来源：http://cvm.jianghu66.top

#endif
来源：http://uxt.c1oappe.top

[S31] C++：Hello World
来源：http://asz.jyoumei.cn


<!-- 参考信息 -->