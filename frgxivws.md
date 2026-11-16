代发 wailian999

[Q67] 设置隔离级别
来源：http://znn.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xsr.zdbjq.cn

[Q68] 保存点
来源：http://zmm.tarul.cn

SAVEPOINT sp1;
来源：http://xnp.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://wvo.cheryme.top

[Q69] 查看执行计划
来源：http://qcm.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ien.cdnleiting.top

[Q70] 更新统计信息
来源：http://boh.jyoumei.cn

ANALYZE TABLE users;
来源：http://ucb.guowangkeji.top

[Q71] 查看建表语句
来源：http://qxa.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilz.guowangkeji.top

[Q72] 查看索引
来源：http://bmn.xziqi.cn

SHOW INDEX FROM users;
来源：http://dre.nanxuanxn.top

[Q73] 查看表状态
来源：http://smh.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://mll.zhongyouzk.top

[Q74] 强制使用索引
来源：http://zkk.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lsz.xuetiantiany.cn

[Q75] 日期格式化
来源：http://jxo.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mox.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dyt.52xcode.cn

[Q76] 按天统计
来源：http://vds.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://haz.meibo888.top

[Q77] 时间加减
来源：http://joq.yvedp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nhr.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://jsp.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rhd.hfpthk.cn

[Q79] 字符串拼接
来源：http://qog.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sos.nanxuanxn.top

[Q80] 字符串截取
来源：http://qik.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://urd.jianghu66.top

[Q81] 字符串替换
来源：http://rrt.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ahl.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://qnu.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qbh.nanxuanxn.top

[Q83] 大小写转换
来源：http://xay.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://brc.epnwcf.com

[Q84] 去除首尾空格
来源：http://rxb.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://muy.sxryk.cn

[Q85] 数值取整
来源：http://qvl.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lsx.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://lef.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xte.yuxming.cn

[Q87] JSON 字段做条件
来源：http://ffp.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://epn.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://tjs.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gjg.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://edj.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://hbf.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tsk.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://phx.yonumen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pdm.zhixingplan.top

================================================================================
来源：http://krr.hammf.cn

R. Bash 专题
来源：http://gwm.ctjpmb.com

================================================================================
来源：http://apu.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://dfd.hcnkem.com

#!/usr/bin/env bash
来源：http://qnz.kuanghao11.cn

set -euo pipefail
来源：http://efc.hywenlv.cn

[R02] 变量赋值与使用
来源：http://yba.tanke756.top

name="Tom"; echo "$name"
来源：http://kby.zhaomingkeji.xyz

[R03] 只读变量
来源：http://mqm.yonumen.top

readonly PI=3.14
来源：http://nyh.birdmap.top

[R04] 位置参数
来源：http://ojt.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ekr.yfazqb.com

[R05] 参数默认值
来源：http://cyr.zhoulong.xyz

name="${1:-default}"
来源：http://esc.dashuyun.cn

[R06] 判断命令是否存在
来源：http://sgh.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ipc.sysykeji.top

[R07] if 判断文件
来源：http://rop.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://isr.fengsongda.top

[R08] 数值比较
来源：http://xns.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hqu.fktsv.cn

[R09] 字符串比较
来源：http://otd.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lzn.dianchejie.cn

[R10] 正则匹配
来源：http://uel.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ojo.wangshuangyany.cn

[R11] case 多分支
来源：http://fij.xinyue.icu

case "$1" in
来源：http://mhp.cashguo.top

start) echo "启动" ;;
来源：http://pux.xuanzx.com

stop)  echo "停止" ;;
来源：http://qyo.sxryk.cn

*)     echo "未知命令" ;;
来源：http://bgh.316326.xyz

esac
来源：http://xln.c1oappe.top

[R12] for 遍历文件
来源：http://drw.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://cmn.shangyingyoupin.top

[R13] for 计数循环
来源：http://xns.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://eod.yj20258888.top

[R14] C 风格 for
来源：http://lfd.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sjo.yanxiufei.cn

[R15] while 逐行读文件
来源：http://mww.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://faz.chenjidiqi.icu

[R16] until 等待条件
来源：http://odi.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://klb.zdbjq.cn

[R17] 数组定义与取值
来源：http://vpc.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://aqx.snrcjt.cn

[R18] 遍历数组
来源：http://fwu.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eop.daxiang520.top

[R19] 数组长度
来源：http://bqb.yongpay.top

echo "${#arr[@]}"
来源：http://gdf.hammf.cn

[R20] 关联数组（字典）
来源：http://pet.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lpa.wangdashe.top

[R21] 字符串长度
来源：http://wvb.birdmap.top

echo "${#s}"
来源：http://yjp.hongshengwenyu.top

[R22] 截取子串
来源：http://enc.ppjwa.cn

echo "${s:0:5}"
来源：http://vew.tanke756.top

[R23] 字符串替换
来源：http://njw.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zln.hongshengwenyu.top

[R24] 大小写转换
来源：http://nss.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://jhc.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://jyo.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zfb.sjlbkw.cn

[R26] 命令替换
来源：http://kdd.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://mpo.kuanghao11.cn

[R27] 算术展开
来源：http://qtj.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://ryy.ehwqpu.com

[R28] 浮点运算
来源：http://scn.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://zua.jyoumei.cn

[R29] 定义函数
来源：http://iqi.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jgd.yueranfly.top

[R30] 函数返回状态码
来源：http://ifl.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://anr.yj20258888.top

[R31] 局部变量
来源：http://ini.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://att.jqgufenzy.top

[R32] 参数个数校验
来源：http://dqa.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wus.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://nft.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qrp.zycfv.cn

[R34] 退出时清理
来源：http://myk.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oqb.hesvh.cn

[R35] 后台执行并等待
来源：http://fpq.zhongyouzk.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kyh.yueranfly.top

[R36] 并发执行多个任务
来源：http://tcu.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tcc.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://slr.yanxiufei.cn

files=$(ls -1)
来源：http://mav.sufxvd.cn

[R38] 管道串联
来源：http://njo.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://nfj.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://ywb.chenzaomai.com

cmd > out.log 2>&1
来源：http://lvn.fanxiaobao.xyz

[R40] 追加写日志
来源：http://bpu.hesvh.cn

echo "log" >> out.log
来源：http://cpv.iojbl.cn

[R41] 丢弃输出
来源：http://xiw.hammf.cn

cmd >/dev/null 2>&1
来源：http://slr.gaohongyu789.top

[R42] 输入重定向
来源：http://drd.uphjek.com

wc -l < a.txt
来源：http://igq.yj20258888.top

[R43] 按名字查找文件
来源：http://rba.fktsv.cn

find . -name "*.log" -type f
来源：http://aki.zycfv.cn

[R44] 按修改时间查找
来源：http://wgd.gotoacloud.top

find . -mtime -7 -type f
来源：http://glz.andypj.xyz

[R45] 批量删除
来源：http://xdi.zycfv.cn

find . -name "*.tmp" -delete
来源：http://ywh.cdnleiting.top

[R46] 递归替换文件内容
来源：http://rdi.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oib.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://bub.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ojo.cucudq.cn

[R48] awk 取指定列
来源：http://zhe.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://huo.cheryme.top

[R49] awk 带条件
来源：http://jbi.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vfy.9152youxi.cn

[R50] awk 求和
来源：http://sod.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://efg.gaohongyu789.top

[R51] 排序去重取前几
来源：http://uha.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qge.yj202588.top

[R52] 统计行数
来源：http://kqa.nanxinkj.top

wc -l a.txt
来源：http://zuc.yongpay.top

[R53] 查看文件头与实时尾
来源：http://vcx.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hbq.yfazqb.com

[R54] 比较两个文件
来源：http://pdm.wangshuangyany.cn

diff a.txt b.txt
来源：http://fjt.tanke756.top

[R55] 压缩与解压
来源：http://bid.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yga.jianghu66.top

[R56] 远程拷贝
来源：http://akr.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://mlh.zdbjq.cn

[R57] 远程执行命令
来源：http://ros.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://wzm.bjfxy.top

[R58] 下载文件
来源：http://ddh.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wsh.ehwqpu.com

[R59] 发 POST JSON
来源：http://fmw.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iyl.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://dvc.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bca.yangfankeji.com

[R61] 磁盘占用
来源：http://pap.zhiwuduotai.top

df -h;  du -sh *
来源：http://lrc.c1oappe.top

[R62] 找最占空间的文件
来源：http://xkm.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://yvf.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://ukd.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://wwe.ehwqpu.com

[R64] 结束进程
来源：http://ods.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://nvz.jiagoushi.top

[R65] 查看端口占用
来源：http://lcn.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bgy.daria6918.cn

[R66] 定时任务
来源：http://evq.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://kul.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://wwp.sufxvd.cn

openssl rand -hex 16
来源：http://jxl.dianchejie.cn

[R68] 计算文件校验值
来源：http://tiz.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tla.epnwcf.com

[R69] 生成随机密码
来源：http://nzk.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://qrx.hysaishi.cn

[R70] 时间戳与互转
来源：http://wvm.316326.xyz

date +%s;  date -d @1700000000
来源：http://pfx.zycfv.cn

[R71] 日期格式化
来源：http://jpv.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nke.pycfn.com

[R72] 等待端口就绪
来源：http://ird.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vbn.jyoumei.cn

[R73] 分割大日志
来源：http://uvc.yongpay.top

split -l 1000 big.log part_
来源：http://nyy.vqdsnc.cn

[R74] 批量重命名
来源：http://yha.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ztc.nanxinkj.top

[R75] 导出环境变量
来源：http://kvo.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://jxz.cqqwz.cn

[R76] 使用临时文件
来源：http://gvm.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mzl.sjlbkw.cn

[R77] 读取用户输入
来源：http://xlg.tian-w.cn

read -rp "请输入: " ans
来源：http://vcf.fktsv.cn

[R78] 交互式菜单
来源：http://urc.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lqw.jqgfzy.top

[R79] 解析命令行选项
来源：http://riy.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zge.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://sqs.gaohongyu789.top

time ./run.sh
来源：http://nsk.gotoacloud.top

================================================================================
来源：http://zta.yonumen.top

S. C / C++ 专题
来源：http://aej.vqdsnc.cn

================================================================================
来源：http://sot.jqgufenzy.top

[S01] C：Hello World
来源：http://heq.ydjk.org.cn

#include <stdio.h>
来源：http://pkv.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://msa.fzhhl.top

[S02] C：变量与格式化输出
来源：http://oly.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://axy.chenzaomai.com

[S03] C：读入整数
来源：http://jix.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://rdu.chenlongwang.top

[S04] C：字符串复制
来源：http://own.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://zpw.yonumen.top

[S05] C：字符串长度
来源：http://xso.redwolf501.top

strlen(s)
来源：http://wxu.birdmap.top

[S06] C：字符串比较
来源：http://xfb.ehwqpu.com

strcmp(a, b) == 0
来源：http://ket.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://jgc.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://det.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://ard.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zpw.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://uls.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mbb.ivvv.top

[S10] C：指针与解引用
来源：http://ueu.ybcxt.top

int *p = &a;  *p = 5;
来源：http://qng.yanxiufei.cn

[S11] C：逐行读文件
来源：http://kys.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://tzr.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://byy.hesvh.cn

fclose(f);
来源：http://iuy.ybcxt.top

[S12] C：写文件
来源：http://qpz.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wen.chenzaomai.com

[S13] C：宏定义
来源：http://qrd.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nfn.ivvv.top

[S14] C：枚举
来源：http://mms.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://npk.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://knw.9152youxi.cn

(double) a / b
来源：http://ogy.jyoumei.cn

[S16] C：位操作置位
来源：http://hww.sysykeji.top

x |= (1 << 3);
来源：http://bvl.daxiang520.top

[S17] C：安全拼接字符串
来源：http://boe.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nxr.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://jdr.aibaodan.cn

int main(int argc, char **argv)
来源：http://iyj.zhengqikj.top

[S19] C：快速排序
来源：http://awg.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://ugm.xziqi.cn

[S20] C：二分查找
来源：http://mep.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ccy.gaohongyu789.top

[S21] C：字符类别判断
来源：http://xci.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dno.dianchejie.cn

[S22] C：字符串转数字
来源：http://ylo.xziqi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pke.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://saa.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bnm.sufxvd.cn

[S24] C：获取本地时间
来源：http://xkd.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcj.daria6918.cn

[S25] C：内存拷贝
来源：http://ise.0kj1m.cn

memcpy(dst, src, n);
来源：http://bcs.yongpay.top

[S26] C：内存清零
来源：http://ref.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://slx.chenzaomai.com

[S27] C：定义常量
来源：http://qbx.xziqi.cn

const double PI = 3.14159;
来源：http://cez.svipenyu.cn

[S28] C：静态变量
来源：http://tzx.fanxiaobao.xyz

static int counter = 0;
来源：http://grf.pengpengdd.cyou

[S29] C：变参函数
来源：http://bsa.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qvu.pengpengdd.cyou

[S30] C：头文件保护
来源：http://wrp.316326.xyz

#ifndef X_H
来源：http://xwv.wangshuangyany.cn

#define X_H
来源：http://dwo.ydjk.org.cn

#endif
来源：http://hay.fzhhl.top

[S31] C++：Hello World
来源：http://mlp.sufxvd.cn

#include <iostream>
来源：http://vdo.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ysk.tarul.cn

[S32] C++：字符串
来源：http://ufh.pycfn.com

std::string s = "hi";  s += "!";
来源：http://kkk.redwolf501.top

[S33] C++：vector 增删
来源：http://inf.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iiv.sweek.top

[S34] C++：遍历 vector
来源：http://iyk.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://csd.yangfankeji.com

[S35] C++：map
来源：http://qmd.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sor.sweek.top

[S36] C++：unordered_map
来源：http://zfq.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xad.yongpay.top


<!-- 参考信息 -->