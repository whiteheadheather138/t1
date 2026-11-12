代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ard.jqgufenzy.top

[Q58] 累计求和
来源：http://wpy.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://puh.c1oappe.top

[Q59] 分组内累计
来源：http://zsw.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgo.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://gqb.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aau.pycfn.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zsb.jinghuilouyu.cn

[Q61] 移动平均
来源：http://cdi.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sxl.jinghuilouyu.cn

[Q62] 分组占比
来源：http://fdz.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lme.haohaochexian.top

[Q63] 开启事务
来源：http://uqx.zdbjq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ktr.havefunace.top

[Q64] 提交事务
来源：http://eco.hnxiangtu.top

COMMIT;
来源：http://wgx.yangfankeji.com

[Q65] 回滚事务
来源：http://qxj.kuanghao11.cn

ROLLBACK;
来源：http://bng.tian-w.cn

[Q66] 行锁查询
来源：http://eqc.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xwu.fengsongda.top

[Q67] 设置隔离级别
来源：http://jyf.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://axc.fzhhl.top

[Q68] 保存点
来源：http://dzj.yfazqb.com

SAVEPOINT sp1;
来源：http://rme.0kj1m.cn

ROLLBACK TO sp1;
来源：http://krt.jqgfzy.top

[Q69] 查看执行计划
来源：http://cxp.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oxz.zhoulong.xyz

[Q70] 更新统计信息
来源：http://elb.cucudq.cn

ANALYZE TABLE users;
来源：http://hkk.quarkkingdee.top

[Q71] 查看建表语句
来源：http://yga.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lfg.nwbrower.top

[Q72] 查看索引
来源：http://jzf.smart0.xyz

SHOW INDEX FROM users;
来源：http://hvm.yj20258.top

[Q73] 查看表状态
来源：http://qmi.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gth.0kj1m.cn

[Q74] 强制使用索引
来源：http://plg.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gyq.cdnleiting.top

[Q75] 日期格式化
来源：http://hzl.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zoc.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kli.xuetiantiany.cn

[Q76] 按天统计
来源：http://ysh.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijs.tianlin.xyz

[Q77] 时间加减
来源：http://pwp.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yuh.jianghu66.top

[Q78] 当前时间
来源：http://aoh.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://guq.yangfankeji.com

[Q79] 字符串拼接
来源：http://wjg.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jgf.uphjek.com

[Q80] 字符串截取
来源：http://cup.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://efv.sjlbkw.cn

[Q81] 字符串替换
来源：http://rej.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://prq.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://aku.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sbm.snrcjt.cn

[Q83] 大小写转换
来源：http://zxz.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://enk.redwolf501.top

[Q84] 去除首尾空格
来源：http://swb.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://jxo.xinyue.icu

[Q85] 数值取整
来源：http://vrd.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kqk.cheryme.top

[Q86] 读取 JSON 字段
来源：http://fal.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ffv.yj20258888.top

[Q87] JSON 字段做条件
来源：http://svo.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pfl.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://rqm.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://reb.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://clh.hammf.cn

[Q89] 判断表是否存在
来源：http://krw.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xbf.yueranfly.top

[Q90] 生成序号列
来源：http://jqj.mhx1999.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eii.chenlongwang.top

================================================================================
来源：http://gwz.vehdjk.com

R. Bash 专题
来源：http://wmq.bbcook.cn

================================================================================
来源：http://azv.52xcode.cn

[R01] shebang 与严格模式
来源：http://zgu.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://jmu.xinyue.icu

set -euo pipefail
来源：http://xop.yfazqb.com

[R02] 变量赋值与使用
来源：http://rlv.dianchejie.cn

name="Tom"; echo "$name"
来源：http://hlp.sufxvd.cn

[R03] 只读变量
来源：http://zes.cashguo.top

readonly PI=3.14
来源：http://ozs.zhiwuduotai.top

[R04] 位置参数
来源：http://gaf.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://anz.jqgufenzy.top

[R05] 参数默认值
来源：http://bfu.hammf.cn

name="${1:-default}"
来源：http://srb.meibo888.top

[R06] 判断命令是否存在
来源：http://cih.zhengqikj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://phq.gaohongyu789.top

[R07] if 判断文件
来源：http://gea.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bej.316326.xyz

[R08] 数值比较
来源：http://hlz.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rpk.yvedp.cn

[R09] 字符串比较
来源：http://jws.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://whu.zhongyouzk.top

[R10] 正则匹配
来源：http://vlv.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ldu.svipenyu.cn

[R11] case 多分支
来源：http://oac.hnqzz.top

case "$1" in
来源：http://hif.aizwys.cn

start) echo "启动" ;;
来源：http://eoa.bjfxy.top

stop)  echo "停止" ;;
来源：http://yqj.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://edu.daxiang520.top

esac
来源：http://bdl.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://bud.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://rrx.fktsv.cn

[R13] for 计数循环
来源：http://ond.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://yhz.cheryme.top

[R14] C 风格 for
来源：http://zce.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lhx.hfpthk.cn

[R15] while 逐行读文件
来源：http://ywe.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kyb.feifeiyinyue.top

[R16] until 等待条件
来源：http://cmv.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://drs.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://qke.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://pec.shangyingyoupin.top

[R18] 遍历数组
来源：http://cot.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rwl.hywenlv.cn

[R19] 数组长度
来源：http://ftz.tianlin.xyz

echo "${#arr[@]}"
来源：http://boe.fehbvm.com

[R20] 关联数组（字典）
来源：http://kaz.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://awb.cdnleiting.top

[R21] 字符串长度
来源：http://wbn.sweek.top

echo "${#s}"
来源：http://xgw.aizwys.cn

[R22] 截取子串
来源：http://kxf.zhiwuduotai.top

echo "${s:0:5}"
来源：http://xgz.sysykeji.top

[R23] 字符串替换
来源：http://lcc.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aza.sxryk.cn

[R24] 大小写转换
来源：http://dwt.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://hkn.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://dlx.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uxz.iojbl.cn

[R26] 命令替换
来源：http://oif.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://eqi.tanke756.top

[R27] 算术展开
来源：http://vsx.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://vha.daxiang520.top

[R28] 浮点运算
来源：http://kos.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://bve.wangshuangyany.cn

[R29] 定义函数
来源：http://uss.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zuj.sysykeji.top

[R30] 函数返回状态码
来源：http://ziq.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://som.haohaochexian.top

[R31] 局部变量
来源：http://brr.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://cgy.birdmap.top

[R32] 参数个数校验
来源：http://kij.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgp.yj20258.top

[R33] 捕获错误并提示行号
来源：http://liz.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jjv.gogol.net.cn

[R34] 退出时清理
来源：http://rbb.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://tic.xylfe.cn

[R35] 后台执行并等待
来源：http://ifr.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://phh.gogol.net.cn

[R36] 并发执行多个任务
来源：http://uiv.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wgi.cucudq.cn

[R37] 把输出赋给变量
来源：http://zfz.cqqwz.cn

files=$(ls -1)
来源：http://khe.sufxvd.cn

[R38] 管道串联
来源：http://nba.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://bvr.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://qok.jinqigufen.top

cmd > out.log 2>&1
来源：http://gtw.xuanzx.com

[R40] 追加写日志
来源：http://dis.jqgufenzy.top

echo "log" >> out.log
来源：http://rie.yvedp.cn

[R41] 丢弃输出
来源：http://tak.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://xhh.zhixingplan.top

[R42] 输入重定向
来源：http://fmf.nwbrower.top

wc -l < a.txt
来源：http://yer.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://oaw.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://dhf.mhx1999.top

[R44] 按修改时间查找
来源：http://eap.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://uhg.cucudq.cn

[R45] 批量删除
来源：http://ilu.vqdsnc.cn

find . -name "*.tmp" -delete
来源：http://tdo.havefunace.top

[R46] 递归替换文件内容
来源：http://lrj.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vpx.guannengcc.top

[R47] sed 单行替换
来源：http://lfo.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ify.gotoacloud.top

[R48] awk 取指定列
来源：http://isa.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://srh.yj20258.top

[R49] awk 带条件
来源：http://gvg.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jsv.zhaomingkeji.xyz

[R50] awk 求和
来源：http://mhv.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://jbc.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://flc.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mos.9152youxi.cn

[R52] 统计行数
来源：http://drt.zycfv.cn

wc -l a.txt
来源：http://ipc.uphjek.com

[R53] 查看文件头与实时尾
来源：http://xjl.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cfj.ppjwa.cn

[R54] 比较两个文件
来源：http://pfk.tianlin.xyz

diff a.txt b.txt
来源：http://mrf.fengsongda.top

[R55] 压缩与解压
来源：http://tsw.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dpc.havefunace.top

[R56] 远程拷贝
来源：http://her.hesvh.cn

scp file user@host:/path/
来源：http://why.zhixingplan.top

[R57] 远程执行命令
来源：http://vhs.aizwys.cn

ssh user@host 'uptime'
来源：http://hrz.cheryme.top

[R58] 下载文件
来源：http://bsd.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://igw.ivvv.top

[R59] 发 POST JSON
来源：http://zvq.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wop.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://uzx.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xrj.wangshuangyany.cn

[R61] 磁盘占用
来源：http://xqg.yonumen.top

df -h;  du -sh *
来源：http://dpj.yj20258.top

[R62] 找最占空间的文件
来源：http://mkl.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://pbp.xuetiantiany.cn

[R63] 内存与进程
来源：http://qkk.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://mrt.gaohongyu789.top

[R64] 结束进程
来源：http://how.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://lqx.chenlongwang.top

[R65] 查看端口占用
来源：http://bmf.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fil.shangyingyoupin.top

[R66] 定时任务
来源：http://cft.jiagoushi.top

crontab -e;  crontab -l
来源：http://ooj.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://gda.pengpengdd.cyou

openssl rand -hex 16
来源：http://tvi.mhx1999.top

[R68] 计算文件校验值
来源：http://frr.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://aou.ctjpmb.com

[R69] 生成随机密码
来源：http://bcu.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://spe.aibaodan.cn

[R70] 时间戳与互转
来源：http://ldc.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://cam.yonumen.top

[R71] 日期格式化
来源：http://mos.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://myu.sufxvd.cn

[R72] 等待端口就绪
来源：http://xwy.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://wyx.chenlongwang.top

[R73] 分割大日志
来源：http://npr.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://hqe.ydzc1.top

[R74] 批量重命名
来源：http://kkw.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gjj.nanxinkj.top

[R75] 导出环境变量
来源：http://jde.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://lng.yuxming.cn

[R76] 使用临时文件
来源：http://fxs.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cho.kuanghao11.cn

[R77] 读取用户输入
来源：http://nkv.yuanzhike.top

read -rp "请输入: " ans
来源：http://kwo.epnwcf.com

[R78] 交互式菜单
来源：http://okc.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uoj.sjlbkw.cn

[R79] 解析命令行选项
来源：http://utz.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kdu.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://fvh.kuanghao11.cn

time ./run.sh
来源：http://aqg.guowangkeji.top

================================================================================
来源：http://qnu.zycfv.cn

S. C / C++ 专题
来源：http://uzz.yuxming.cn

================================================================================
来源：http://khk.yanxiufei.cn

[S01] C：Hello World
来源：http://keq.zhongyouzk.top

#include <stdio.h>
来源：http://ngx.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydn.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://gae.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://mzx.ivvv.top

[S03] C：读入整数
来源：http://viw.yj20258888.top

int x; scanf("%d", &x);
来源：http://xte.ybcxt.top

[S04] C：字符串复制
来源：http://fbe.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ztv.tanke756.top

[S05] C：字符串长度
来源：http://rsq.ctjpmb.com

strlen(s)
来源：http://gud.xuanzx.com

[S06] C：字符串比较
来源：http://nqh.guowangkeji.top

strcmp(a, b) == 0
来源：http://gbf.birdmap.top

[S07] C：数组遍历求和
来源：http://znf.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yhh.cashguo.top

[S08] C：动态内存分配与释放
来源：http://xnx.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ggo.uphjek.com

[S09] C：结构体定义与初始化
来源：http://gmg.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yqx.kuanghao11.cn

[S10] C：指针与解引用
来源：http://lwo.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://vsm.nwbrower.top

[S11] C：逐行读文件
来源：http://shi.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://dtq.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hgt.shuidangran.top

fclose(f);
来源：http://vqg.andypj.xyz

[S12] C：写文件
来源：http://nsh.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqw.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://adi.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hnu.bjfxy.top

[S14] C：枚举
来源：http://wds.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://xbn.chenjidiqi.icu

[S15] C：类型转换
来源：http://dvt.shzxlz.cn

(double) a / b
来源：http://tdi.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://gsp.yj20258888.top

x |= (1 << 3);
来源：http://jno.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://yse.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pqy.fzhhl.top

[S18] C：命令行参数
来源：http://ola.tarul.cn

int main(int argc, char **argv)
来源：http://fnh.cdnleiting.top

[S19] C：快速排序
来源：http://xoo.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://akc.bjfxy.top

[S20] C：二分查找
来源：http://gzm.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jct.gogol.net.cn

[S21] C：字符类别判断
来源：http://ntn.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qtw.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://tjg.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hat.hywenlv.cn

[S23] C：随机数
来源：http://zfv.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ues.ctjpmb.com

[S24] C：获取本地时间
来源：http://wub.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nur.fzhhl.top

[S25] C：内存拷贝
来源：http://atp.jinqigfzy.top

memcpy(dst, src, n);
来源：http://srj.sweek.top

[S26] C：内存清零
来源：http://yql.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://ylk.quarkkingdee.top

[S27] C：定义常量
来源：http://fgd.sweek.top

const double PI = 3.14159;
来源：http://ecn.fanxiaobao.xyz

[S28] C：静态变量
来源：http://wvc.daxiang520.top


<!-- 参考信息 -->