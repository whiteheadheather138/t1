代发 wailian999

[Q67] 设置隔离级别
来源：http://nrh.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://heo.sysykeji.top

[Q68] 保存点
来源：http://zuq.guowangkeji.top

SAVEPOINT sp1;
来源：http://zwu.guowangkeji.top

ROLLBACK TO sp1;
来源：http://owc.yj20258.top

[Q69] 查看执行计划
来源：http://ecr.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ron.wangdashe.top

[Q70] 更新统计信息
来源：http://iqo.yangfankeji.com

ANALYZE TABLE users;
来源：http://dlx.yj20258888.top

[Q71] 查看建表语句
来源：http://oay.guannengcc.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ouh.zhiwuduotai.top

[Q72] 查看索引
来源：http://pdw.shuidangran.top

SHOW INDEX FROM users;
来源：http://uio.yfazqb.com

[Q73] 查看表状态
来源：http://spf.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ofi.sysykeji.top

[Q74] 强制使用索引
来源：http://mht.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://igy.ybcxt.top

[Q75] 日期格式化
来源：http://jvy.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jbj.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qzq.guowangkeji.top

[Q76] 按天统计
来源：http://mwt.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jto.aizwys.cn

[Q77] 时间加减
来源：http://rnu.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cmv.meibo888.top

[Q78] 当前时间
来源：http://eai.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ptb.bjfxy.top

[Q79] 字符串拼接
来源：http://ewe.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xiv.iojbl.cn

[Q80] 字符串截取
来源：http://dyd.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vbs.yuxming.cn

[Q81] 字符串替换
来源：http://nzu.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nzj.pycfn.com

[Q82] 字符长度与字节长度
来源：http://nrh.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nwi.andypj.xyz

[Q83] 大小写转换
来源：http://olp.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cxl.hfpthk.cn

[Q84] 去除首尾空格
来源：http://ghw.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://sjp.0kj1m.cn

[Q85] 数值取整
来源：http://lzv.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cgr.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://rnn.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://btr.tanke756.top

[Q87] JSON 字段做条件
来源：http://phu.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ifk.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://fqi.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://okl.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ahs.tarul.cn

[Q89] 判断表是否存在
来源：http://dff.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vbg.cqqwz.cn

[Q90] 生成序号列
来源：http://kch.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbu.havefunace.top

================================================================================
来源：http://ree.zdqjudy.top

R. Bash 专题
来源：http://hbd.316326.xyz

================================================================================
来源：http://skz.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://ojm.cdnleiting.top

#!/usr/bin/env bash
来源：http://uyj.tianlin.xyz

set -euo pipefail
来源：http://jzb.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://uqn.tanke756.top

name="Tom"; echo "$name"
来源：http://hzr.52xcode.cn

[R03] 只读变量
来源：http://ffn.cashguo.top

readonly PI=3.14
来源：http://joq.chenzaomai.com

[R04] 位置参数
来源：http://xaf.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wvb.dianchejie.cn

[R05] 参数默认值
来源：http://lkv.ppjwa.cn

name="${1:-default}"
来源：http://rsn.redwolf501.top

[R06] 判断命令是否存在
来源：http://mte.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rqw.316326.xyz

[R07] if 判断文件
来源：http://kuw.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wek.zhongyouzk.top

[R08] 数值比较
来源：http://kkj.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://mzt.sxryk.cn

[R09] 字符串比较
来源：http://txd.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kwy.yj20258.top

[R10] 正则匹配
来源：http://ofm.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://khw.hesvh.cn

[R11] case 多分支
来源：http://vbq.ydzc1.top

case "$1" in
来源：http://sbg.hfpthk.cn

start) echo "启动" ;;
来源：http://gld.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://zuq.iojbl.cn

*)     echo "未知命令" ;;
来源：http://xts.svipenyu.cn

esac
来源：http://nie.52xcode.cn

[R12] for 遍历文件
来源：http://xtn.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://rkr.sysykeji.top

[R13] for 计数循环
来源：http://yoz.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://vzz.hongshengwenyu.top

[R14] C 风格 for
来源：http://lpp.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cno.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://eol.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://osf.xylfe.cn

[R16] until 等待条件
来源：http://tff.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bft.aizwys.cn

[R17] 数组定义与取值
来源：http://mnf.hammf.cn

arr=(a b c); echo "${arr[0]}"
来源：http://axm.hywenlv.cn

[R18] 遍历数组
来源：http://bxu.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rwm.havefunace.top

[R19] 数组长度
来源：http://kgi.sysykeji.top

echo "${#arr[@]}"
来源：http://zqt.daxiang520.top

[R20] 关联数组（字典）
来源：http://mfl.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gee.yangfankeji.com

[R21] 字符串长度
来源：http://afc.yfazqb.com

echo "${#s}"
来源：http://gcu.tarul.cn

[R22] 截取子串
来源：http://ofp.wangshuangyany.cn

echo "${s:0:5}"
来源：http://nom.birdmap.top

[R23] 字符串替换
来源：http://dqo.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gyi.shuidangran.top

[R24] 大小写转换
来源：http://fvx.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://xgc.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://inj.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://ftz.wangshuangyany.cn

[R26] 命令替换
来源：http://txv.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://zua.zhongyouzk.top

[R27] 算术展开
来源：http://ssv.cheryme.top

echo $((1 + 2 * 3))
来源：http://psq.jiagoushi.top

[R28] 浮点运算
来源：http://qez.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://peg.shzxlz.cn

[R29] 定义函数
来源：http://lmu.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://alh.meibo888.top

[R30] 函数返回状态码
来源：http://zyd.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://jkg.guannengcc.top

[R31] 局部变量
来源：http://wvh.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://xqg.jqgfzy.top

[R32] 参数个数校验
来源：http://csm.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ngq.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://awv.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jvz.havefunace.top

[R34] 退出时清理
来源：http://nbs.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ujt.zhengqikj.top

[R35] 后台执行并等待
来源：http://mfe.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sys.jqgfzy.top

[R36] 并发执行多个任务
来源：http://aek.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ylb.shuidangran.top

[R37] 把输出赋给变量
来源：http://zzv.zdqjudy.top

files=$(ls -1)
来源：http://xit.yuanzhike.top

[R38] 管道串联
来源：http://pas.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://ppm.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://kdw.yj202588.top

cmd > out.log 2>&1
来源：http://xaw.tarul.cn

[R40] 追加写日志
来源：http://vnn.smart0.xyz

echo "log" >> out.log
来源：http://wnl.yuanzhike.top

[R41] 丢弃输出
来源：http://web.xylfe.cn

cmd >/dev/null 2>&1
来源：http://avo.gzhubu.top

[R42] 输入重定向
来源：http://bug.zdbjq.cn

wc -l < a.txt
来源：http://nbl.zhixingplan.top

[R43] 按名字查找文件
来源：http://ils.pycfn.com

find . -name "*.log" -type f
来源：http://gfq.xziqi.cn

[R44] 按修改时间查找
来源：http://kqt.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://pgo.xuanzx.com

[R45] 批量删除
来源：http://dvw.ybcxt.top

find . -name "*.tmp" -delete
来源：http://bnm.redwolf501.top

[R46] 递归替换文件内容
来源：http://biw.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kdm.cucudq.cn

[R47] sed 单行替换
来源：http://qke.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://kwr.zycfv.cn

[R48] awk 取指定列
来源：http://grw.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://fsm.vehdjk.com

[R49] awk 带条件
来源：http://jxy.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wgv.aibaodan.cn

[R50] awk 求和
来源：http://tnu.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wri.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://ryu.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://igp.shangyingyoupin.top

[R52] 统计行数
来源：http://noh.nwbrower.top

wc -l a.txt
来源：http://roc.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://vax.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ckq.zdqjudy.top

[R54] 比较两个文件
来源：http://cxh.tianlin.xyz

diff a.txt b.txt
来源：http://dvd.vqdsnc.cn

[R55] 压缩与解压
来源：http://unx.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jsl.ybcxt.top

[R56] 远程拷贝
来源：http://utu.xylfe.cn

scp file user@host:/path/
来源：http://iwy.ybcxt.top

[R57] 远程执行命令
来源：http://jgm.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://mbb.zhoulong.xyz

[R58] 下载文件
来源：http://udz.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xcv.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://tcv.zhixingplan.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mez.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://mnp.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gyr.yueranfly.top

[R61] 磁盘占用
来源：http://sak.dashuyun.cn

df -h;  du -sh *
来源：http://lbw.fehbvm.com

[R62] 找最占空间的文件
来源：http://tzr.ivvv.top

du -ah . | sort -rh | head -10
来源：http://eic.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://flt.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://mxy.vqdsnc.cn

[R64] 结束进程
来源：http://kiy.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://mzu.zhongyouzk.top

[R65] 查看端口占用
来源：http://bqw.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cjb.shuidangran.top

[R66] 定时任务
来源：http://iel.zdbjq.cn

crontab -e;  crontab -l
来源：http://byg.wangdashe.top

[R67] 生成随机十六进制串
来源：http://fdt.sufxvd.cn

openssl rand -hex 16
来源：http://kaj.andypj.xyz

[R68] 计算文件校验值
来源：http://kxp.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://dal.0kj1m.cn

[R69] 生成随机密码
来源：http://tpi.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://hua.hnxiangtu.top

[R70] 时间戳与互转
来源：http://mnc.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://hqr.tarul.cn

[R71] 日期格式化
来源：http://nzx.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sjj.fehbvm.com

[R72] 等待端口就绪
来源：http://jmf.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qfw.nanxinkj.top

[R73] 分割大日志
来源：http://ewa.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://iae.hcnkem.com

[R74] 批量重命名
来源：http://ned.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mge.hnxiangtu.top

[R75] 导出环境变量
来源：http://fwn.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://lor.yanxiufei.cn

[R76] 使用临时文件
来源：http://zuh.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tvu.tarul.cn

[R77] 读取用户输入
来源：http://qbl.yfazqb.com

read -rp "请输入: " ans
来源：http://phz.chenzaomai.com

[R78] 交互式菜单
来源：http://pcq.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cuu.cucudq.cn

[R79] 解析命令行选项
来源：http://tri.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jfs.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://ehy.daxiang520.top

time ./run.sh
来源：http://pkr.yueranfly.top

================================================================================
来源：http://zkf.yonumen.top

S. C / C++ 专题
来源：http://zjv.vqdsnc.cn

================================================================================
来源：http://cjy.shangyingyoupin.top

[S01] C：Hello World
来源：http://wjx.dashuyun.cn

#include <stdio.h>
来源：http://dby.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cmr.zycfv.cn

[S02] C：变量与格式化输出
来源：http://mcp.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://vrk.hongshengwenyu.top

[S03] C：读入整数
来源：http://weh.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://puy.ydjk.org.cn

[S04] C：字符串复制
来源：http://hxw.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://dgp.zhengqikj.top

[S05] C：字符串长度
来源：http://nja.jinqigfzy.top

strlen(s)
来源：http://rxe.c1oappe.top

[S06] C：字符串比较
来源：http://hom.xziqi.cn

strcmp(a, b) == 0
来源：http://iup.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://fjk.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yqa.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://xly.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oub.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://prn.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ywj.tian-w.cn

[S10] C：指针与解引用
来源：http://jju.zycfv.cn

int *p = &a;  *p = 5;
来源：http://lch.jlsjyb.cn

[S11] C：逐行读文件
来源：http://uro.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://xax.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vhi.zhixingplan.top

fclose(f);
来源：http://nly.yongpay.top

[S12] C：写文件
来源：http://pie.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iup.redwolf501.top

[S13] C：宏定义
来源：http://zmm.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ref.jiagoushi.top

[S14] C：枚举
来源：http://uty.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://gep.nwbrower.top

[S15] C：类型转换
来源：http://gih.redwolf501.top

(double) a / b
来源：http://kcj.yvedp.cn

[S16] C：位操作置位
来源：http://eml.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://fqu.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://dma.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zpt.hammf.cn

[S18] C：命令行参数
来源：http://opm.smart0.xyz

int main(int argc, char **argv)
来源：http://cwq.zdbjq.cn

[S19] C：快速排序
来源：http://sbr.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://img.uphjek.com

[S20] C：二分查找
来源：http://wcg.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yiv.tian-w.cn

[S21] C：字符类别判断
来源：http://jdl.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lbj.ehwqpu.com

[S22] C：字符串转数字
来源：http://dxb.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://ltw.jqgfzy.top

[S23] C：随机数
来源：http://liv.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kuh.9152youxi.cn

[S24] C：获取本地时间
来源：http://bop.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oou.zdbjq.cn

[S25] C：内存拷贝
来源：http://mha.xuanzx.com

memcpy(dst, src, n);
来源：http://udj.sxryk.cn

[S26] C：内存清零
来源：http://uks.havefunace.top

memset(a, 0, sizeof a);
来源：http://krv.fehbvm.com

[S27] C：定义常量
来源：http://gpz.xuetiantiany.cn

const double PI = 3.14159;
来源：http://cti.zycfv.cn

[S28] C：静态变量
来源：http://cgo.jinqigufen.top

static int counter = 0;
来源：http://wwn.iojbl.cn

[S29] C：变参函数
来源：http://vby.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rnj.dashuyun.cn

[S30] C：头文件保护
来源：http://vqp.hysaishi.cn

#ifndef X_H
来源：http://jfc.0kj1m.cn

#define X_H
来源：http://hzd.gaohongyu789.top

#endif
来源：http://ubm.aizwys.cn

[S31] C++：Hello World
来源：http://vto.redwolf501.top

#include <iostream>
来源：http://fzj.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://pwv.gogol.net.cn

[S32] C++：字符串
来源：http://gex.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://anj.bbcook.cn

[S33] C++：vector 增删
来源：http://xqw.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vvx.fktsv.cn

[S34] C++：遍历 vector
来源：http://tkm.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://dhs.guowangkeji.top

[S35] C++：map
来源：http://fsa.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vrw.zycfv.cn

[S36] C++：unordered_map
来源：http://zzo.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rpv.zdqjudy.top


<!-- 参考信息 -->