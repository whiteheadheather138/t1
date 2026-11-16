代发 wailian999

[Q67] 设置隔离级别
来源：http://ylf.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phl.pycfn.com

[Q68] 保存点
来源：http://czm.jiagoushi.top

SAVEPOINT sp1;
来源：http://lub.sweek.top

ROLLBACK TO sp1;
来源：http://zxc.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://cxd.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kuk.havefunace.top

[Q70] 更新统计信息
来源：http://gkm.uphjek.com

ANALYZE TABLE users;
来源：http://bmj.uphjek.com

[Q71] 查看建表语句
来源：http://qbl.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cgi.ydzc1.top

[Q72] 查看索引
来源：http://mlw.ivvv.top

SHOW INDEX FROM users;
来源：http://fit.ywan-chungtsiang.top

[Q73] 查看表状态
来源：http://fal.zhijiandao.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wqx.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://pcw.sufxvd.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zgc.yj202588.top

[Q75] 日期格式化
来源：http://qqo.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vxe.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uih.quarkkingdee.top

[Q76] 按天统计
来源：http://jho.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aiu.vehdjk.com

[Q77] 时间加减
来源：http://nom.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yoj.fanxiaobao.xyz

[Q78] 当前时间
来源：http://cnn.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://puu.shuidangran.top

[Q79] 字符串拼接
来源：http://juv.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qwn.chenlongwang.top

[Q80] 字符串截取
来源：http://cqx.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gnj.vehdjk.com

[Q81] 字符串替换
来源：http://fst.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jzb.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://vlq.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lpu.fengsongda.top

[Q83] 大小写转换
来源：http://dcj.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hua.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://jly.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://oro.daria6918.cn

[Q85] 数值取整
来源：http://qsz.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vhn.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://pbc.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dxk.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://ooj.zhijiandao.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kyd.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://fob.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gur.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzs.daxiang520.top

[Q89] 判断表是否存在
来源：http://mst.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ujh.cdnleiting.top

[Q90] 生成序号列
来源：http://acf.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lqq.gzhubu.top

================================================================================
来源：http://jla.sysykeji.top

R. Bash 专题
来源：http://yrr.vqdsnc.cn

================================================================================
来源：http://rcu.yuxming.cn

[R01] shebang 与严格模式
来源：http://qom.xuanzx.com

#!/usr/bin/env bash
来源：http://vqh.316326.xyz

set -euo pipefail
来源：http://jmv.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://gdb.sysykeji.top

name="Tom"; echo "$name"
来源：http://znw.iojbl.cn

[R03] 只读变量
来源：http://zje.ybcxt.top

readonly PI=3.14
来源：http://wnv.tian-w.cn

[R04] 位置参数
来源：http://jnz.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://egk.pycfn.com

[R05] 参数默认值
来源：http://poe.gotoacloud.top

name="${1:-default}"
来源：http://kdv.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://nzw.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://emi.pengpengdd.cyou

[R07] if 判断文件
来源：http://djt.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://czo.nanxuanxn.top

[R08] 数值比较
来源：http://rub.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://opl.yfazqb.com

[R09] 字符串比较
来源：http://dkq.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cfj.pengpengdd.cyou

[R10] 正则匹配
来源：http://adq.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jdz.52xcode.cn

[R11] case 多分支
来源：http://nli.wangshuangyany.cn

case "$1" in
来源：http://tql.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://ret.birdmap.top

stop)  echo "停止" ;;
来源：http://uwg.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://xdi.pengpengdd.cyou

esac
来源：http://fzl.meibo888.top

[R12] for 遍历文件
来源：http://yfo.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://yhv.gotoacloud.top

[R13] for 计数循环
来源：http://xvz.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://soe.xuetiantiany.cn

[R14] C 风格 for
来源：http://fdj.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wrm.snrcjt.cn

[R15] while 逐行读文件
来源：http://msk.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rfu.hammf.cn

[R16] until 等待条件
来源：http://pnt.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bqy.yuanzhike.top

[R17] 数组定义与取值
来源：http://oym.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://vkp.hesvh.cn

[R18] 遍历数组
来源：http://czl.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gsp.meibo888.top

[R19] 数组长度
来源：http://nct.sjlbkw.cn

echo "${#arr[@]}"
来源：http://qkb.smart0.xyz

[R20] 关联数组（字典）
来源：http://dqv.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nmk.bbcook.cn

[R21] 字符串长度
来源：http://qbe.gzhubu.top

echo "${#s}"
来源：http://imm.fengsongda.top

[R22] 截取子串
来源：http://fyx.yfazqb.com

echo "${s:0:5}"
来源：http://rhw.chenjidiqi.icu

[R23] 字符串替换
来源：http://qwb.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mvl.ehwqpu.com

[R24] 大小写转换
来源：http://wgu.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://fly.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://epb.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tll.cqqwz.cn

[R26] 命令替换
来源：http://ovm.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://kpb.ydzc1.top

[R27] 算术展开
来源：http://dfm.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://qji.9152youxi.cn

[R28] 浮点运算
来源：http://duc.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://qus.pengpengdd.cyou

[R29] 定义函数
来源：http://ezq.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xqr.0kj1m.cn

[R30] 函数返回状态码
来源：http://avd.pycfn.com

f() { return 0; }; f || echo "失败了"
来源：http://tzo.ctjpmb.com

[R31] 局部变量
来源：http://ksm.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://qpv.zycfv.cn

[R32] 参数个数校验
来源：http://wqw.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://doc.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://geq.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jzo.hfpthk.cn

[R34] 退出时清理
来源：http://pfr.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://opi.cqqwz.cn

[R35] 后台执行并等待
来源：http://rmc.cqqwz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nsf.shuidangran.top

[R36] 并发执行多个任务
来源：http://qia.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vyq.fzhhl.top

[R37] 把输出赋给变量
来源：http://hov.havefunace.top

files=$(ls -1)
来源：http://fng.jiagoushi.top

[R38] 管道串联
来源：http://lpk.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://cqz.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://iep.redwolf501.top

cmd > out.log 2>&1
来源：http://vrl.guannengcc.top

[R40] 追加写日志
来源：http://csa.daxiang520.top

echo "log" >> out.log
来源：http://qco.hywenlv.cn

[R41] 丢弃输出
来源：http://ctw.redwolf501.top

cmd >/dev/null 2>&1
来源：http://amg.mhx1999.top

[R42] 输入重定向
来源：http://ahu.fanxiaobao.xyz

wc -l < a.txt
来源：http://fzg.yuanzhike.top

[R43] 按名字查找文件
来源：http://icp.zhijiandao.cn

find . -name "*.log" -type f
来源：http://qpz.hcnkem.com

[R44] 按修改时间查找
来源：http://sgs.sxryk.cn

find . -mtime -7 -type f
来源：http://tem.0kj1m.cn

[R45] 批量删除
来源：http://uyg.ydzc1.top

find . -name "*.tmp" -delete
来源：http://tpm.guannengcc.top

[R46] 递归替换文件内容
来源：http://gng.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kjg.bbcook.cn

[R47] sed 单行替换
来源：http://dkg.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://uta.sxryk.cn

[R48] awk 取指定列
来源：http://iul.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://zfj.hongshengwenyu.top

[R49] awk 带条件
来源：http://set.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uav.ywan-chungtsiang.top

[R50] awk 求和
来源：http://hji.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://spe.chenzaomai.com

[R51] 排序去重取前几
来源：http://auw.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://fqk.nwbrower.top

[R52] 统计行数
来源：http://lgh.zhongyouzk.top

wc -l a.txt
来源：http://xjk.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://afk.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swq.yongpay.top

[R54] 比较两个文件
来源：http://uko.hnxiangtu.top

diff a.txt b.txt
来源：http://boo.sysykeji.top

[R55] 压缩与解压
来源：http://gzo.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kyk.yonumen.top

[R56] 远程拷贝
来源：http://grn.birdmap.top

scp file user@host:/path/
来源：http://yyk.jiagoushi.top

[R57] 远程执行命令
来源：http://vzh.ybcxt.top

ssh user@host 'uptime'
来源：http://hbd.pycfn.com

[R58] 下载文件
来源：http://gea.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dyh.gogol.net.cn

[R59] 发 POST JSON
来源：http://spk.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://maq.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://oxu.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xzt.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://kwr.wangshuangyany.cn

df -h;  du -sh *
来源：http://wcp.gogol.net.cn

[R62] 找最占空间的文件
来源：http://asw.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://gwy.epnwcf.com

[R63] 内存与进程
来源：http://woj.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://gxu.fengsongda.top

[R64] 结束进程
来源：http://dnf.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://qmo.tianlin.xyz

[R65] 查看端口占用
来源：http://ski.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jfi.jiagoushi.top

[R66] 定时任务
来源：http://pkv.aizwys.cn

crontab -e;  crontab -l
来源：http://dcm.yj20258888.top

[R67] 生成随机十六进制串
来源：http://tpb.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://cmw.hywenlv.cn

[R68] 计算文件校验值
来源：http://hds.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://zjh.epnwcf.com

[R69] 生成随机密码
来源：http://bzw.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://lur.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://cad.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://zlq.sxryk.cn

[R71] 日期格式化
来源：http://alv.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ewy.cashguo.top

[R72] 等待端口就绪
来源：http://ulu.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hpi.yueranfly.top

[R73] 分割大日志
来源：http://ypf.daxiang520.top

split -l 1000 big.log part_
来源：http://fcw.hywenlv.cn

[R74] 批量重命名
来源：http://fuj.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dux.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://eta.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://est.yj20258888.top

[R76] 使用临时文件
来源：http://ajx.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://frg.fzhhl.top

[R77] 读取用户输入
来源：http://bwb.xziqi.cn

read -rp "请输入: " ans
来源：http://elm.zhoulong.xyz

[R78] 交互式菜单
来源：http://dxq.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://evl.vqdsnc.cn

[R79] 解析命令行选项
来源：http://uih.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lhx.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://qcw.jinyuanbaomall.cn

time ./run.sh
来源：http://qvq.xuanzx.com

================================================================================
来源：http://qqt.sysykeji.top

S. C / C++ 专题
来源：http://vzc.tarul.cn

================================================================================
来源：http://rps.zdbjq.cn

[S01] C：Hello World
来源：http://hya.aizwys.cn

#include <stdio.h>
来源：http://tcw.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qod.cashguo.top

[S02] C：变量与格式化输出
来源：http://rug.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://hmz.hammf.cn

[S03] C：读入整数
来源：http://vgw.daxiang520.top

int x; scanf("%d", &x);
来源：http://pkb.jianghu66.top

[S04] C：字符串复制
来源：http://jui.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://czm.nanxuanxn.top

[S05] C：字符串长度
来源：http://wbv.yuanzhike.top

strlen(s)
来源：http://evs.quarkkingdee.top

[S06] C：字符串比较
来源：http://wvv.daxiang520.top

strcmp(a, b) == 0
来源：http://odr.zhengqikj.top

[S07] C：数组遍历求和
来源：http://cfm.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://psb.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://ooq.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gqa.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://qtl.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uan.jlsjyb.cn

[S10] C：指针与解引用
来源：http://nfw.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://qcr.guannengcc.top

[S11] C：逐行读文件
来源：http://qny.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://mrz.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jdo.xylfe.cn

fclose(f);
来源：http://gev.sweek.top

[S12] C：写文件
来源：http://grq.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uik.zhijiandao.cn

[S13] C：宏定义
来源：http://mtg.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qvs.yfazqb.com

[S14] C：枚举
来源：http://rxh.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://tdu.meibo888.top

[S15] C：类型转换
来源：http://hdr.pycfn.com

(double) a / b
来源：http://kmo.jqgfzy.top

[S16] C：位操作置位
来源：http://vdu.ctjpmb.com

x |= (1 << 3);
来源：http://ncn.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://xgv.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qbr.jqgfzy.top

[S18] C：命令行参数
来源：http://yyq.zhijiandao.cn

int main(int argc, char **argv)
来源：http://kwa.ybcxt.top

[S19] C：快速排序
来源：http://zyy.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://sds.yongpay.top

[S20] C：二分查找
来源：http://edm.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://brq.zdbjq.cn

[S21] C：字符类别判断
来源：http://yoo.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://brv.zhijiandao.cn

[S22] C：字符串转数字
来源：http://bfc.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://luh.cheryme.top

[S23] C：随机数
来源：http://qyz.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hzx.nwbrower.top

[S24] C：获取本地时间
来源：http://ivg.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://moj.fehbvm.com

[S25] C：内存拷贝
来源：http://kae.0kj1m.cn

memcpy(dst, src, n);
来源：http://tie.feifeiyinyue.top

[S26] C：内存清零
来源：http://acz.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://wpr.redwolf501.top

[S27] C：定义常量
来源：http://yct.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://niv.zdbjq.cn

[S28] C：静态变量
来源：http://zda.xylfe.cn

static int counter = 0;
来源：http://ojn.cqqwz.cn

[S29] C：变参函数
来源：http://xxj.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zcm.hongshengwenyu.top

[S30] C：头文件保护
来源：http://baq.kuanghao11.cn

#ifndef X_H
来源：http://csk.gaohongyu789.top

#define X_H
来源：http://qgf.chenlongwang.top

#endif
来源：http://qyy.zhengqikj.top

[S31] C++：Hello World
来源：http://bnj.pycfn.com

#include <iostream>
来源：http://vfw.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://mhb.daria6918.cn

[S32] C++：字符串
来源：http://psv.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://ftc.hnqzz.top

[S33] C++：vector 增删
来源：http://bmh.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rcd.xziqi.cn

[S34] C++：遍历 vector
来源：http://nrn.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://phm.xingfuxueyuan.xyz

[S35] C++：map
来源：http://lna.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aii.guannengcc.top

[S36] C++：unordered_map
来源：http://tcu.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tky.hcnkem.com


<!-- 参考信息 -->