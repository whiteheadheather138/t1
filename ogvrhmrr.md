代发 wailian999

ROLLBACK TO sp1;
来源：http://axd.ybcxt.top

[Q69] 查看执行计划
来源：http://ole.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iyn.ehwqpu.com

[Q70] 更新统计信息
来源：http://kql.9152youxi.cn

ANALYZE TABLE users;
来源：http://vqp.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://ixu.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://opx.feifeiyinyue.top

[Q72] 查看索引
来源：http://mjh.cucudq.cn

SHOW INDEX FROM users;
来源：http://uoc.andypj.xyz

[Q73] 查看表状态
来源：http://tym.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ifz.birdmap.top

[Q74] 强制使用索引
来源：http://ohq.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pyp.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://jwl.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cnb.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dfp.bbcook.cn

[Q76] 按天统计
来源：http://ote.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xmr.fanxiaobao.xyz

[Q77] 时间加减
来源：http://mqr.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qrl.zhixingplan.top

[Q78] 当前时间
来源：http://rfz.shanyushiyangtech.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifc.bjfxy.top

[Q79] 字符串拼接
来源：http://dgd.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://djz.hcnkem.com

[Q80] 字符串截取
来源：http://cpq.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lol.nanxuanxn.top

[Q81] 字符串替换
来源：http://fef.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oac.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://qhj.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gnj.zhoulong.xyz

[Q83] 大小写转换
来源：http://aba.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://otf.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://cvo.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://aap.vehdjk.com

[Q85] 数值取整
来源：http://ena.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ahv.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://eev.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://udy.cdnleiting.top

[Q87] JSON 字段做条件
来源：http://vrf.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fox.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://xpe.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://asf.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tab.zdbjq.cn

[Q89] 判断表是否存在
来源：http://dlk.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ghd.52xcode.cn

[Q90] 生成序号列
来源：http://qhf.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bcy.yvedp.cn

================================================================================
来源：http://bef.cheryme.top

R. Bash 专题
来源：http://cig.jiagoushi.top

================================================================================
来源：http://mhb.cheryme.top

[R01] shebang 与严格模式
来源：http://rhy.cqqwz.cn

#!/usr/bin/env bash
来源：http://yrf.shuidangran.top

set -euo pipefail
来源：http://yky.fktsv.cn

[R02] 变量赋值与使用
来源：http://rup.bjfxy.top

name="Tom"; echo "$name"
来源：http://wls.quarkkingdee.top

[R03] 只读变量
来源：http://fzf.gogol.net.cn

readonly PI=3.14
来源：http://tvc.hesvh.cn

[R04] 位置参数
来源：http://qas.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hsi.jinqigfzy.top

[R05] 参数默认值
来源：http://wxo.birdmap.top

name="${1:-default}"
来源：http://rqg.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://tll.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sxh.zdbjq.cn

[R07] if 判断文件
来源：http://zqj.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jbq.yongpay.top

[R08] 数值比较
来源：http://dyk.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://clf.cqqwz.cn

[R09] 字符串比较
来源：http://jhj.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ftv.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://avq.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rub.guowangkeji.top

[R11] case 多分支
来源：http://knc.gogol.net.cn

case "$1" in
来源：http://fww.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://snc.zhixingplan.top

stop)  echo "停止" ;;
来源：http://adp.nanxuanxn.top

*)     echo "未知命令" ;;
来源：http://gmo.nwbrower.top

esac
来源：http://lip.hfpthk.cn

[R12] for 遍历文件
来源：http://uvl.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://lse.sufxvd.cn

[R13] for 计数循环
来源：http://huf.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://ems.bjfxy.top

[R14] C 风格 for
来源：http://shq.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gza.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://zce.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ypj.yuanzhike.top

[R16] until 等待条件
来源：http://rta.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ozq.ydjk.org.cn

[R17] 数组定义与取值
来源：http://zvq.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://nni.jqgufenzy.top

[R18] 遍历数组
来源：http://apo.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bvh.chenlongwang.top

[R19] 数组长度
来源：http://cii.sysykeji.top

echo "${#arr[@]}"
来源：http://epl.uphjek.com

[R20] 关联数组（字典）
来源：http://yok.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hqr.vehdjk.com

[R21] 字符串长度
来源：http://jap.chenzaomai.com

echo "${#s}"
来源：http://mzr.yueranfly.top

[R22] 截取子串
来源：http://nwd.yonumen.top

echo "${s:0:5}"
来源：http://jdl.shuidangran.top

[R23] 字符串替换
来源：http://zll.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://woz.bjfxy.top

[R24] 大小写转换
来源：http://abb.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://dpm.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://lev.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qsm.yonumen.top

[R26] 命令替换
来源：http://vxf.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://zlq.dianchejie.cn

[R27] 算术展开
来源：http://pcd.ybcxt.top

echo $((1 + 2 * 3))
来源：http://ect.shuidangran.top

[R28] 浮点运算
来源：http://bxo.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://nqo.zhoulong.xyz

[R29] 定义函数
来源：http://ziz.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iwm.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://fqe.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://bvg.hfpthk.cn

[R31] 局部变量
来源：http://abc.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://kal.dashuyun.cn

[R32] 参数个数校验
来源：http://dmh.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pxg.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://inx.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kcp.cucudq.cn

[R34] 退出时清理
来源：http://hdf.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rwn.nwbrower.top

[R35] 后台执行并等待
来源：http://soo.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ajw.nanxinkj.top

[R36] 并发执行多个任务
来源：http://pnt.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://too.yonumen.top

[R37] 把输出赋给变量
来源：http://eqd.chenzaomai.com

files=$(ls -1)
来源：http://ahr.ydjk.org.cn

[R38] 管道串联
来源：http://rjn.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://gif.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://qdf.hammf.cn

cmd > out.log 2>&1
来源：http://sfa.snrcjt.cn

[R40] 追加写日志
来源：http://dek.zdqjudy.top

echo "log" >> out.log
来源：http://vaa.yongpay.top

[R41] 丢弃输出
来源：http://exo.hnqzz.top

cmd >/dev/null 2>&1
来源：http://wcw.shanyushiyangtech.top

[R42] 输入重定向
来源：http://xko.jinghuilouyu.cn

wc -l < a.txt
来源：http://ygu.chenlongwang.top

[R43] 按名字查找文件
来源：http://gxs.sysykeji.top

find . -name "*.log" -type f
来源：http://iir.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://vlk.zdqjudy.top

find . -mtime -7 -type f
来源：http://ufn.fehbvm.com

[R45] 批量删除
来源：http://ldb.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://lwx.tarul.cn

[R46] 递归替换文件内容
来源：http://vkq.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mip.birdmap.top

[R47] sed 单行替换
来源：http://uaf.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sca.nanxuanxn.top

[R48] awk 取指定列
来源：http://bhp.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://llh.meibo888.top

[R49] awk 带条件
来源：http://efa.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tyk.shzxlz.cn

[R50] awk 求和
来源：http://vky.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oko.yongpay.top

[R51] 排序去重取前几
来源：http://whz.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ivf.iojbl.cn

[R52] 统计行数
来源：http://idk.zhijiandao.cn

wc -l a.txt
来源：http://lxl.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://yay.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bac.ehwqpu.com

[R54] 比较两个文件
来源：http://bxh.yueranfly.top

diff a.txt b.txt
来源：http://xce.cucudq.cn

[R55] 压缩与解压
来源：http://pkn.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gxx.mhx1999.top

[R56] 远程拷贝
来源：http://pon.zhixingplan.top

scp file user@host:/path/
来源：http://nto.yangfankeji.com

[R57] 远程执行命令
来源：http://vfh.ybcxt.top

ssh user@host 'uptime'
来源：http://wyx.ywan-chungtsiang.top

[R58] 下载文件
来源：http://mts.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pkq.jqgfzy.top

[R59] 发 POST JSON
来源：http://rti.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ewq.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://syt.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xrt.vehdjk.com

[R61] 磁盘占用
来源：http://hmj.tanke756.top

df -h;  du -sh *
来源：http://igy.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://opd.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://bri.ehwqpu.com

[R63] 内存与进程
来源：http://ngf.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://ixc.wangdashe.top

[R64] 结束进程
来源：http://nja.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://mqr.zdqjudy.top

[R65] 查看端口占用
来源：http://uzv.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tlb.jianghu66.top

[R66] 定时任务
来源：http://sxg.gotoacloud.top

crontab -e;  crontab -l
来源：http://sdu.vehdjk.com

[R67] 生成随机十六进制串
来源：http://ptp.yuxming.cn

openssl rand -hex 16
来源：http://qtr.cashguo.top

[R68] 计算文件校验值
来源：http://srw.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://rsz.hammf.cn

[R69] 生成随机密码
来源：http://umm.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ofp.zhengqikj.top

[R70] 时间戳与互转
来源：http://cqe.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://uwm.ehwqpu.com

[R71] 日期格式化
来源：http://yln.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://epy.sufxvd.cn

[R72] 等待端口就绪
来源：http://tyg.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fin.nanxuanxn.top

[R73] 分割大日志
来源：http://skc.aizwys.cn

split -l 1000 big.log part_
来源：http://zij.ehwqpu.com

[R74] 批量重命名
来源：http://kmq.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nin.ybcxt.top

[R75] 导出环境变量
来源：http://ykl.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://leb.daxiang520.top

[R76] 使用临时文件
来源：http://evt.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mck.tanke756.top

[R77] 读取用户输入
来源：http://bsi.yvedp.cn

read -rp "请输入: " ans
来源：http://zuq.cucudq.cn

[R78] 交互式菜单
来源：http://dfc.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qfz.tarul.cn

[R79] 解析命令行选项
来源：http://wps.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ltu.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://rep.hammf.cn

time ./run.sh
来源：http://uos.zhixingplan.top

================================================================================
来源：http://pvp.fktsv.cn

S. C / C++ 专题
来源：http://wqt.cqqwz.cn

================================================================================
来源：http://arl.9152youxi.cn

[S01] C：Hello World
来源：http://nne.sxryk.cn

#include <stdio.h>
来源：http://uee.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://trg.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://jpq.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://pkr.jianghu66.top

[S03] C：读入整数
来源：http://ygq.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://rez.snrcjt.cn

[S04] C：字符串复制
来源：http://tns.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lxo.vqdsnc.cn

[S05] C：字符串长度
来源：http://ncy.nanxuanxn.top

strlen(s)
来源：http://uof.jqgfzy.top

[S06] C：字符串比较
来源：http://akj.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://czt.xinyue.icu

[S07] C：数组遍历求和
来源：http://sjj.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://exe.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://uwa.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tfu.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://gvt.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vff.uphjek.com

[S10] C：指针与解引用
来源：http://tzh.guannengcc.top

int *p = &a;  *p = 5;
来源：http://knl.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://oip.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://aae.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lqk.hnqzz.top

fclose(f);
来源：http://yjs.nwbrower.top

[S12] C：写文件
来源：http://shk.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ucm.guannengcc.top

[S13] C：宏定义
来源：http://cuw.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pjp.zhengqikj.top

[S14] C：枚举
来源：http://rtm.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://ouu.havefunace.top

[S15] C：类型转换
来源：http://ebe.jqgufenzy.top

(double) a / b
来源：http://hkc.birdmap.top

[S16] C：位操作置位
来源：http://wzi.shuidangran.top

x |= (1 << 3);
来源：http://vya.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://bvz.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lbz.wangdashe.top

[S18] C：命令行参数
来源：http://bcn.sysykeji.top

int main(int argc, char **argv)
来源：http://iry.hnqzz.top

[S19] C：快速排序
来源：http://mlf.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://zxt.yongpay.top

[S20] C：二分查找
来源：http://pel.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lsv.hywenlv.cn

[S21] C：字符类别判断
来源：http://nfd.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rmc.yonumen.top

[S22] C：字符串转数字
来源：http://lhj.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ztn.pycfn.com

[S23] C：随机数
来源：http://jdv.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://egy.sweek.top

[S24] C：获取本地时间
来源：http://khb.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ckg.ivvv.top

[S25] C：内存拷贝
来源：http://wen.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://wlg.tanke756.top

[S26] C：内存清零
来源：http://dpd.vehdjk.com

memset(a, 0, sizeof a);
来源：http://cjm.xuanzx.com

[S27] C：定义常量
来源：http://nrw.hfpthk.cn

const double PI = 3.14159;
来源：http://xim.sxryk.cn

[S28] C：静态变量
来源：http://hmh.c1oappe.top

static int counter = 0;
来源：http://zbh.hnqzz.top

[S29] C：变参函数
来源：http://dsx.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rxe.zdqjudy.top

[S30] C：头文件保护
来源：http://zhb.xziqi.cn

#ifndef X_H
来源：http://ppz.sjlbkw.cn

#define X_H
来源：http://zkf.hysaishi.cn

#endif
来源：http://jfk.gotoacloud.top

[S31] C++：Hello World
来源：http://sfx.zhiwuduotai.top

#include <iostream>
来源：http://efv.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://cln.tianlin.xyz

[S32] C++：字符串
来源：http://bab.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://dny.redwolf501.top

[S33] C++：vector 增删
来源：http://ufk.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bmc.snrcjt.cn

[S34] C++：遍历 vector
来源：http://iex.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://vvv.tanke756.top

[S35] C++：map
来源：http://rco.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywc.tarul.cn

[S36] C++：unordered_map
来源：http://doi.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xew.gaohongyu789.top

[S37] C++：set
来源：http://oof.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gsd.hammf.cn

[S38] C++：排序
来源：http://emz.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://pzl.ehwqpu.com


<!-- 参考信息 -->