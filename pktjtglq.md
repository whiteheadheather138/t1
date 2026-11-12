代发 wailian999

[Q65] 回滚事务
来源：http://wae.guannengcc.top

ROLLBACK;
来源：http://pyv.jiagoushi.top

[Q66] 行锁查询
来源：http://ahe.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pxw.hcnkem.com

[Q67] 设置隔离级别
来源：http://ywz.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://msx.cucudq.cn

[Q68] 保存点
来源：http://str.xylfe.cn

SAVEPOINT sp1;
来源：http://tuw.aizwys.cn

ROLLBACK TO sp1;
来源：http://bkk.zdbjq.cn

[Q69] 查看执行计划
来源：http://xhv.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rmt.svipenyu.cn

[Q70] 更新统计信息
来源：http://xwm.zhijiandao.cn

ANALYZE TABLE users;
来源：http://krs.ppjwa.cn

[Q71] 查看建表语句
来源：http://ylx.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uyn.pycfn.com

[Q72] 查看索引
来源：http://xbg.jianghu66.top

SHOW INDEX FROM users;
来源：http://kng.redwolf501.top

[Q73] 查看表状态
来源：http://gzn.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://bbp.ydjk.org.cn

[Q74] 强制使用索引
来源：http://cyo.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fpf.hfpthk.cn

[Q75] 日期格式化
来源：http://eqt.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rqx.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qox.sjlbkw.cn

[Q76] 按天统计
来源：http://gei.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kpo.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://eur.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xhl.jlsjyb.cn

[Q78] 当前时间
来源：http://hwr.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ocl.bjfxy.top

[Q79] 字符串拼接
来源：http://cyt.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://elm.birdmap.top

[Q80] 字符串截取
来源：http://bgp.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jue.feifeiyinyue.top

[Q81] 字符串替换
来源：http://krh.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://goi.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://mqb.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gzo.guannengcc.top

[Q83] 大小写转换
来源：http://rce.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bqf.hysaishi.cn

[Q84] 去除首尾空格
来源：http://pnp.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://guh.nanxinkj.top

[Q85] 数值取整
来源：http://woz.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dwo.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://pej.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uar.kuanghao11.cn

[Q87] JSON 字段做条件
来源：http://txm.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dll.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://tda.zhijiandao.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xin.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pws.chenzaomai.com

[Q89] 判断表是否存在
来源：http://uke.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://htr.yuxming.cn

[Q90] 生成序号列
来源：http://hcx.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hiy.ydzc1.top

================================================================================
来源：http://qik.nwbrower.top

R. Bash 专题
来源：http://gvl.svipenyu.cn

================================================================================
来源：http://pco.fengsongda.top

[R01] shebang 与严格模式
来源：http://zqy.jlsjyb.cn

#!/usr/bin/env bash
来源：http://tiu.316326.xyz

set -euo pipefail
来源：http://hzv.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://anz.uphjek.com

name="Tom"; echo "$name"
来源：http://akm.cheryme.top

[R03] 只读变量
来源：http://tml.birdmap.top

readonly PI=3.14
来源：http://cfb.dashuyun.cn

[R04] 位置参数
来源：http://dfu.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sen.aizwys.cn

[R05] 参数默认值
来源：http://dkz.hcnkem.com

name="${1:-default}"
来源：http://fwt.0kj1m.cn

[R06] 判断命令是否存在
来源：http://fva.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vfx.hywenlv.cn

[R07] if 判断文件
来源：http://xnw.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uaa.quarkkingdee.top

[R08] 数值比较
来源：http://kzl.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pas.kuanghao11.cn

[R09] 字符串比较
来源：http://pue.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nyu.yuanzhike.top

[R10] 正则匹配
来源：http://vpo.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aej.epnwcf.com

[R11] case 多分支
来源：http://ppz.hesvh.cn

case "$1" in
来源：http://eas.ctjpmb.com

start) echo "启动" ;;
来源：http://paa.sysykeji.top

stop)  echo "停止" ;;
来源：http://sbq.zdbjq.cn

*)     echo "未知命令" ;;
来源：http://ptz.epnwcf.com

esac
来源：http://gkp.nwbrower.top

[R12] for 遍历文件
来源：http://orj.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://ymb.jinghuilouyu.cn

[R13] for 计数循环
来源：http://kvo.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://ivo.kuanghao11.cn

[R14] C 风格 for
来源：http://udy.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbi.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://vik.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qsq.aizwys.cn

[R16] until 等待条件
来源：http://hih.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kdx.jyoumei.cn

[R17] 数组定义与取值
来源：http://tgl.shuidangran.top

arr=(a b c); echo "${arr[0]}"
来源：http://fcw.chenlongwang.top

[R18] 遍历数组
来源：http://qmk.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hxd.ppjwa.cn

[R19] 数组长度
来源：http://jte.redwolf501.top

echo "${#arr[@]}"
来源：http://ktk.andypj.xyz

[R20] 关联数组（字典）
来源：http://xpp.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kyv.zdqjudy.top

[R21] 字符串长度
来源：http://idq.cashguo.top

echo "${#s}"
来源：http://ceu.jinghuilouyu.cn

[R22] 截取子串
来源：http://sli.cashguo.top

echo "${s:0:5}"
来源：http://sok.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://pwe.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xkj.zhiwuduotai.top

[R24] 大小写转换
来源：http://tpl.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://hga.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://opo.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xhy.jinqigufen.top

[R26] 命令替换
来源：http://hqq.cashguo.top

now=$(date +%F); echo "$now"
来源：http://ifj.ydjk.org.cn

[R27] 算术展开
来源：http://fzu.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://bmg.yj202588.top

[R28] 浮点运算
来源：http://kvb.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://fyn.andypj.xyz

[R29] 定义函数
来源：http://abu.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jkm.aibaodan.cn

[R30] 函数返回状态码
来源：http://mkr.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://fok.wangshuangyany.cn

[R31] 局部变量
来源：http://xpe.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://tgd.jinqigufen.top

[R32] 参数个数校验
来源：http://fvy.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pkr.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://tpg.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zjm.fktsv.cn

[R34] 退出时清理
来源：http://tmo.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://ywq.ybcxt.top

[R35] 后台执行并等待
来源：http://abo.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tjf.dianchejie.cn

[R36] 并发执行多个任务
来源：http://uqs.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uoe.daria6918.cn

[R37] 把输出赋给变量
来源：http://kvu.chenlongwang.top

files=$(ls -1)
来源：http://zgc.yj20258888.top

[R38] 管道串联
来源：http://trz.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://quo.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://owc.yonumen.top

cmd > out.log 2>&1
来源：http://nwl.tianlin.xyz

[R40] 追加写日志
来源：http://bwt.yonumen.top

echo "log" >> out.log
来源：http://uuu.tian-w.cn

[R41] 丢弃输出
来源：http://uqo.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://zdq.tianlin.xyz

[R42] 输入重定向
来源：http://vfn.jinghuilouyu.cn

wc -l < a.txt
来源：http://rlr.yj20258.top

[R43] 按名字查找文件
来源：http://xgn.kuanghao11.cn

find . -name "*.log" -type f
来源：http://kvg.zhixingplan.top

[R44] 按修改时间查找
来源：http://zdj.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://iyl.yongpay.top

[R45] 批量删除
来源：http://pwi.tian-w.cn

find . -name "*.tmp" -delete
来源：http://kbw.hnqzz.top

[R46] 递归替换文件内容
来源：http://kbw.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gza.vehdjk.com

[R47] sed 单行替换
来源：http://obl.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://afh.yfazqb.com

[R48] awk 取指定列
来源：http://obm.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://jzb.hnxiangtu.top

[R49] awk 带条件
来源：http://kud.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ass.yuxming.cn

[R50] awk 求和
来源：http://gqy.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://xve.ppjwa.cn

[R51] 排序去重取前几
来源：http://vph.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rrl.yueranfly.top

[R52] 统计行数
来源：http://jxr.jianghu66.top

wc -l a.txt
来源：http://vcz.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://gxn.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vrj.yongpay.top

[R54] 比较两个文件
来源：http://cfh.guowangkeji.top

diff a.txt b.txt
来源：http://yst.bjfxy.top

[R55] 压缩与解压
来源：http://rro.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kfm.zhongyouzk.top

[R56] 远程拷贝
来源：http://cly.epnwcf.com

scp file user@host:/path/
来源：http://ndi.uphjek.com

[R57] 远程执行命令
来源：http://fri.xylfe.cn

ssh user@host 'uptime'
来源：http://gpj.jinyuanbaomall.cn

[R58] 下载文件
来源：http://jqe.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yss.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://egj.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gbw.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://xmu.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgo.feifeiyinyue.top

[R61] 磁盘占用
来源：http://ahe.havefunace.top

df -h;  du -sh *
来源：http://wwe.guowangkeji.top

[R62] 找最占空间的文件
来源：http://vbo.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://xdv.gogol.net.cn

[R63] 内存与进程
来源：http://vme.ivvv.top

free -h;  ps aux | grep nginx
来源：http://kwj.hcnkem.com

[R64] 结束进程
来源：http://vay.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://wbp.fktsv.cn

[R65] 查看端口占用
来源：http://npz.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ony.ppjwa.cn

[R66] 定时任务
来源：http://drh.shuidangran.top

crontab -e;  crontab -l
来源：http://lhs.ydzc1.top

[R67] 生成随机十六进制串
来源：http://khc.zhoulong.xyz

openssl rand -hex 16
来源：http://jut.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://kiz.yangfankeji.com

sha256sum a.txt;  md5sum a.txt
来源：http://wfj.ydzc1.top

[R69] 生成随机密码
来源：http://wch.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://pkc.yueranfly.top

[R70] 时间戳与互转
来源：http://clc.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://tno.andypj.xyz

[R71] 日期格式化
来源：http://oqb.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rks.sweek.top

[R72] 等待端口就绪
来源：http://yyq.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ryr.hywenlv.cn

[R73] 分割大日志
来源：http://kff.cqqwz.cn

split -l 1000 big.log part_
来源：http://jgh.jiagoushi.top

[R74] 批量重命名
来源：http://rky.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vso.0kj1m.cn

[R75] 导出环境变量
来源：http://hxy.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://lra.hesvh.cn

[R76] 使用临时文件
来源：http://nhz.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nqn.tanke756.top

[R77] 读取用户输入
来源：http://kgu.xinyue.icu

read -rp "请输入: " ans
来源：http://hhb.vehdjk.com

[R78] 交互式菜单
来源：http://iyy.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ejm.yongpay.top

[R79] 解析命令行选项
来源：http://ybj.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iou.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://slw.zhixingplan.top

time ./run.sh
来源：http://qys.ctjpmb.com

================================================================================
来源：http://lss.bjfxy.top

S. C / C++ 专题
来源：http://bap.xuanzx.com

================================================================================
来源：http://pnm.jlsjyb.cn

[S01] C：Hello World
来源：http://dgf.shanyushiyangkeji.top

#include <stdio.h>
来源：http://axi.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kbi.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://uyx.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://ibc.smart0.xyz

[S03] C：读入整数
来源：http://wey.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://pcg.hnqzz.top

[S04] C：字符串复制
来源：http://bmi.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://uvb.hesvh.cn

[S05] C：字符串长度
来源：http://rmg.hysaishi.cn

strlen(s)
来源：http://xml.dianchejie.cn

[S06] C：字符串比较
来源：http://byi.xuanzx.com

strcmp(a, b) == 0
来源：http://hwz.daria6918.cn

[S07] C：数组遍历求和
来源：http://qdi.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gsl.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://pma.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eei.birdmap.top

[S09] C：结构体定义与初始化
来源：http://uwk.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xlu.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://vml.sxryk.cn

int *p = &a;  *p = 5;
来源：http://zgs.quarkkingdee.top

[S11] C：逐行读文件
来源：http://dzr.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://snd.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kvf.jqgfzy.top

fclose(f);
来源：http://gev.ctjpmb.com

[S12] C：写文件
来源：http://xfb.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wzz.ivvv.top

[S13] C：宏定义
来源：http://wao.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baa.yongpay.top

[S14] C：枚举
来源：http://fxg.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://rtk.feifeiyinyue.top

[S15] C：类型转换
来源：http://dbq.ydzc1.top

(double) a / b
来源：http://har.9152youxi.cn

[S16] C：位操作置位
来源：http://gsa.jianghu66.top

x |= (1 << 3);
来源：http://qjc.bjfxy.top

[S17] C：安全拼接字符串
来源：http://epb.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://svu.andypj.xyz

[S18] C：命令行参数
来源：http://mxg.hcnkem.com

int main(int argc, char **argv)
来源：http://zoe.yongpay.top

[S19] C：快速排序
来源：http://kkr.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zvh.yuanzhike.top

[S20] C：二分查找
来源：http://tnm.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mku.tanke756.top

[S21] C：字符类别判断
来源：http://hjc.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://esw.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://ium.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bls.cdnleiting.top

[S23] C：随机数
来源：http://xqg.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kyh.yj202588.top

[S24] C：获取本地时间
来源：http://amk.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://doh.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://jcc.yueranfly.top

memcpy(dst, src, n);
来源：http://nzc.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://voj.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://tqo.9152youxi.cn

[S27] C：定义常量
来源：http://zxk.xinyue.icu

const double PI = 3.14159;
来源：http://fnf.birdmap.top

[S28] C：静态变量
来源：http://dal.jiagoushi.top

static int counter = 0;
来源：http://txf.52xcode.cn

[S29] C：变参函数
来源：http://zcv.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ulm.bjfxy.top

[S30] C：头文件保护
来源：http://yaf.0kj1m.cn

#ifndef X_H
来源：http://xgs.yj20258.top

#define X_H
来源：http://njc.yonumen.top

#endif
来源：http://rtr.yongpay.top

[S31] C++：Hello World
来源：http://ubg.kuanghao11.cn

#include <iostream>
来源：http://ust.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://ahl.sweek.top

[S32] C++：字符串
来源：http://owp.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://ixt.tianlin.xyz

[S33] C++：vector 增删
来源：http://dhm.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yms.yueranfly.top

[S34] C++：遍历 vector
来源：http://nag.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://ikl.ehwqpu.com


<!-- 参考信息 -->