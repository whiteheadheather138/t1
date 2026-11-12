代发 wailian999

ROLLBACK TO sp1;
来源：http://asy.zycfv.cn

[Q69] 查看执行计划
来源：http://jwq.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vyy.pycfn.com

[Q70] 更新统计信息
来源：http://abi.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://cax.fengsongda.top

[Q71] 查看建表语句
来源：http://jui.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vmx.jlsjyb.cn

[Q72] 查看索引
来源：http://ful.yj20258.top

SHOW INDEX FROM users;
来源：http://sjz.bjfxy.top

[Q73] 查看表状态
来源：http://ycg.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://chb.hcnkem.com

[Q74] 强制使用索引
来源：http://xqu.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uyb.aizwys.cn

[Q75] 日期格式化
来源：http://jrs.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uzf.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bdl.jinqigufen.top

[Q76] 按天统计
来源：http://ptf.hnqzz.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://klg.zhixingplan.top

[Q77] 时间加减
来源：http://eoh.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wye.yongpay.top

[Q78] 当前时间
来源：http://myv.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ktg.zdqjudy.top

[Q79] 字符串拼接
来源：http://lix.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://msf.tianlin.xyz

[Q80] 字符串截取
来源：http://ahh.fehbvm.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pgp.haohaochexian.top

[Q81] 字符串替换
来源：http://ffz.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ohh.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://ptf.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwo.daxiang520.top

[Q83] 大小写转换
来源：http://zii.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cdd.chenlongwang.top

[Q84] 去除首尾空格
来源：http://ecy.zhaomingkeji.xyz

SELECT TRIM(name) FROM users;
来源：http://jgm.gaohongyu789.top

[Q85] 数值取整
来源：http://kpp.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ben.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://hqo.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://htw.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://ucz.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kgi.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://xzm.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xca.vqdsnc.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdn.wangdashe.top

[Q89] 判断表是否存在
来源：http://ixo.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ldk.svipenyu.cn

[Q90] 生成序号列
来源：http://hgn.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rkd.chenjidiqi.icu

================================================================================
来源：http://wma.zycfv.cn

R. Bash 专题
来源：http://wrq.meibo888.top

================================================================================
来源：http://mel.0kj1m.cn

[R01] shebang 与严格模式
来源：http://dam.0kj1m.cn

#!/usr/bin/env bash
来源：http://jqt.gotoacloud.top

set -euo pipefail
来源：http://tzu.jiagoushi.top

[R02] 变量赋值与使用
来源：http://eju.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://gni.tianlin.xyz

[R03] 只读变量
来源：http://zaj.sxryk.cn

readonly PI=3.14
来源：http://gjx.tianlin.xyz

[R04] 位置参数
来源：http://udn.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rsi.cucudq.cn

[R05] 参数默认值
来源：http://fcw.zdqjudy.top

name="${1:-default}"
来源：http://hvf.xylfe.cn

[R06] 判断命令是否存在
来源：http://gxw.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rav.iojbl.cn

[R07] if 判断文件
来源：http://jes.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aoq.cucudq.cn

[R08] 数值比较
来源：http://kpe.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lbq.redwolf501.top

[R09] 字符串比较
来源：http://iuk.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yoh.birdmap.top

[R10] 正则匹配
来源：http://xer.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rnc.hysaishi.cn

[R11] case 多分支
来源：http://czf.yongpay.top

case "$1" in
来源：http://hfw.xylfe.cn

start) echo "启动" ;;
来源：http://fxq.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://rzg.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://vyr.cashguo.top

esac
来源：http://jrd.ydzc1.top

[R12] for 遍历文件
来源：http://fpx.yuanzhike.top

for f in *.txt; do echo "$f"; done
来源：http://xwd.birdmap.top

[R13] for 计数循环
来源：http://ruj.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://fhc.cashguo.top

[R14] C 风格 for
来源：http://sbi.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fxr.52xcode.cn

[R15] while 逐行读文件
来源：http://gba.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qgh.iojbl.cn

[R16] until 等待条件
来源：http://etc.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ipz.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://egp.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://hpx.ybcxt.top

[R18] 遍历数组
来源：http://fci.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bsc.haohaochexian.top

[R19] 数组长度
来源：http://vzz.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://ore.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://trm.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ilt.sufxvd.cn

[R21] 字符串长度
来源：http://ziu.zhixingplan.top

echo "${#s}"
来源：http://btt.52xcode.cn

[R22] 截取子串
来源：http://avf.shangyingyoupin.top

echo "${s:0:5}"
来源：http://tjn.gogol.net.cn

[R23] 字符串替换
来源：http://atg.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vmg.shzxlz.cn

[R24] 大小写转换
来源：http://ise.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://khf.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://fyx.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wif.sweek.top

[R26] 命令替换
来源：http://whu.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://vtt.yuxming.cn

[R27] 算术展开
来源：http://sdq.52xcode.cn

echo $((1 + 2 * 3))
来源：http://pkg.wangdashe.top

[R28] 浮点运算
来源：http://dcj.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://ege.wangshuangyany.cn

[R29] 定义函数
来源：http://akm.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aiq.0kj1m.cn

[R30] 函数返回状态码
来源：http://rcc.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://enr.yangfankeji.com

[R31] 局部变量
来源：http://pmd.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://xhz.sxryk.cn

[R32] 参数个数校验
来源：http://nda.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://smn.yongpay.top

[R33] 捕获错误并提示行号
来源：http://pjk.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kqt.zhijiandao.cn

[R34] 退出时清理
来源：http://viu.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://hoi.haohaochexian.top

[R35] 后台执行并等待
来源：http://xoj.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jcj.ybcxt.top

[R36] 并发执行多个任务
来源：http://kfl.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zuk.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://xrg.shangyingyoupin.top

files=$(ls -1)
来源：http://sqo.aizwys.cn

[R38] 管道串联
来源：http://eho.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://nne.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://gfl.redwolf501.top

cmd > out.log 2>&1
来源：http://heu.c1oappe.top

[R40] 追加写日志
来源：http://aos.hammf.cn

echo "log" >> out.log
来源：http://xsr.chenlongwang.top

[R41] 丢弃输出
来源：http://xyw.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://rjs.zhixingplan.top

[R42] 输入重定向
来源：http://cgs.hnqzz.top

wc -l < a.txt
来源：http://fvk.jianghu66.top

[R43] 按名字查找文件
来源：http://hlp.andypj.xyz

find . -name "*.log" -type f
来源：http://vfb.jyoumei.cn

[R44] 按修改时间查找
来源：http://kej.uphjek.com

find . -mtime -7 -type f
来源：http://vuo.gzhubu.top

[R45] 批量删除
来源：http://met.guannengcc.top

find . -name "*.tmp" -delete
来源：http://kpz.havefunace.top

[R46] 递归替换文件内容
来源：http://qnx.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bga.gogol.net.cn

[R47] sed 单行替换
来源：http://vep.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://pkw.svipenyu.cn

[R48] awk 取指定列
来源：http://yru.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://fxk.ydjk.org.cn

[R49] awk 带条件
来源：http://byy.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://esb.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://uhf.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jna.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://wxq.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hzo.jqgufenzy.top

[R52] 统计行数
来源：http://zcr.haohaochexian.top

wc -l a.txt
来源：http://whz.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://rys.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fho.daxiang520.top

[R54] 比较两个文件
来源：http://hak.jiagoushi.top

diff a.txt b.txt
来源：http://cho.yueranfly.top

[R55] 压缩与解压
来源：http://fzd.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mgu.vehdjk.com

[R56] 远程拷贝
来源：http://fij.xinyue.icu

scp file user@host:/path/
来源：http://ogv.bjfxy.top

[R57] 远程执行命令
来源：http://rte.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://mdu.tianlin.xyz

[R58] 下载文件
来源：http://opu.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://omt.cheryme.top

[R59] 发 POST JSON
来源：http://orv.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mnh.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://hsh.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://elh.iojbl.cn

[R61] 磁盘占用
来源：http://pgc.jinghuilouyu.cn

df -h;  du -sh *
来源：http://lcv.jinqigufen.top

[R62] 找最占空间的文件
来源：http://sni.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://wol.tarul.cn

[R63] 内存与进程
来源：http://jpf.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://ndk.jqgfzy.top

[R64] 结束进程
来源：http://hkn.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://ahq.cdnleiting.top

[R65] 查看端口占用
来源：http://icl.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ols.zhixingplan.top

[R66] 定时任务
来源：http://nwt.daria6918.cn

crontab -e;  crontab -l
来源：http://bck.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://kkg.yueranfly.top

openssl rand -hex 16
来源：http://sth.svipenyu.cn

[R68] 计算文件校验值
来源：http://ixu.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cud.fzhhl.top

[R69] 生成随机密码
来源：http://atz.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://mfw.aibaodan.cn

[R70] 时间戳与互转
来源：http://dyn.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://gqq.mhx1999.top

[R71] 日期格式化
来源：http://jss.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://wnu.daria6918.cn

[R72] 等待端口就绪
来源：http://xza.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gol.fehbvm.com

[R73] 分割大日志
来源：http://cfi.redwolf501.top

split -l 1000 big.log part_
来源：http://vng.nanxuanxn.top

[R74] 批量重命名
来源：http://cgq.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://emg.svipenyu.cn

[R75] 导出环境变量
来源：http://wdb.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://tjx.nwbrower.top

[R76] 使用临时文件
来源：http://ebh.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxg.sweek.top

[R77] 读取用户输入
来源：http://ylc.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://xel.chenzaomai.com

[R78] 交互式菜单
来源：http://lvg.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mew.haohaochexian.top

[R79] 解析命令行选项
来源：http://gjr.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pbk.uphjek.com

[R80] 查看脚本执行耗时
来源：http://kuj.epnwcf.com

time ./run.sh
来源：http://tyf.jinqigufen.top

================================================================================
来源：http://lkk.cashguo.top

S. C / C++ 专题
来源：http://rot.shanyushiyangtech.top

================================================================================
来源：http://vml.tian-w.cn

[S01] C：Hello World
来源：http://tlw.uphjek.com

#include <stdio.h>
来源：http://imo.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qjq.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://vwa.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://nxy.daria6918.cn

[S03] C：读入整数
来源：http://rek.tian-w.cn

int x; scanf("%d", &x);
来源：http://vfz.jianghu66.top

[S04] C：字符串复制
来源：http://bkx.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zlj.hysaishi.cn

[S05] C：字符串长度
来源：http://zry.fzhhl.top

strlen(s)
来源：http://edg.fengsongda.top

[S06] C：字符串比较
来源：http://kbo.kuanghao11.cn

strcmp(a, b) == 0
来源：http://xox.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://ier.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tlo.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://aru.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aap.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://cgx.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cxm.hesvh.cn

[S10] C：指针与解引用
来源：http://set.jianghu66.top

int *p = &a;  *p = 5;
来源：http://khl.epnwcf.com

[S11] C：逐行读文件
来源：http://tpy.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://nte.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fvc.vehdjk.com

fclose(f);
来源：http://wto.jqgfzy.top

[S12] C：写文件
来源：http://qpu.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bvn.tanke756.top

[S13] C：宏定义
来源：http://bxd.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kvq.fanxiaobao.xyz

[S14] C：枚举
来源：http://iin.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://deh.cdnleiting.top

[S15] C：类型转换
来源：http://szq.ppjwa.cn

(double) a / b
来源：http://gju.ybcxt.top

[S16] C：位操作置位
来源：http://ady.nanxinkj.top

x |= (1 << 3);
来源：http://tfv.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://bxv.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://unn.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://tss.shuidangran.top

int main(int argc, char **argv)
来源：http://cbt.fanxiaobao.xyz

[S19] C：快速排序
来源：http://wfq.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://rvd.yangfankeji.com

[S20] C：二分查找
来源：http://vig.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mrm.zhengqikj.top

[S21] C：字符类别判断
来源：http://fvp.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://obs.tanke756.top

[S22] C：字符串转数字
来源：http://esb.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jzd.svipenyu.cn

[S23] C：随机数
来源：http://cff.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vyg.uphjek.com

[S24] C：获取本地时间
来源：http://fuy.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cul.yonumen.top

[S25] C：内存拷贝
来源：http://twd.xuanzx.com

memcpy(dst, src, n);
来源：http://hhx.wangdashe.top

[S26] C：内存清零
来源：http://prb.havefunace.top

memset(a, 0, sizeof a);
来源：http://fnm.redwolf501.top

[S27] C：定义常量
来源：http://tqj.havefunace.top

const double PI = 3.14159;
来源：http://okz.pycfn.com

[S28] C：静态变量
来源：http://hkw.aizwys.cn

static int counter = 0;
来源：http://fcu.guowangkeji.top

[S29] C：变参函数
来源：http://fhb.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfn.fktsv.cn

[S30] C：头文件保护
来源：http://ddy.hcnkem.com

#ifndef X_H
来源：http://sap.0kj1m.cn

#define X_H
来源：http://ner.hnxiangtu.top

#endif
来源：http://kqo.sweek.top

[S31] C++：Hello World
来源：http://emb.iojbl.cn

#include <iostream>
来源：http://fzc.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://bxd.yanxiufei.cn

[S32] C++：字符串
来源：http://deq.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://mfu.yuanzhike.top

[S33] C++：vector 增删
来源：http://apf.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mmn.zdbjq.cn

[S34] C++：遍历 vector
来源：http://vhf.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://mjg.vqdsnc.cn

[S35] C++：map
来源：http://qce.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gkp.yuxming.cn

[S36] C++：unordered_map
来源：http://htz.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwb.hnqzz.top

[S37] C++：set
来源：http://roh.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qdt.dianchejie.cn

[S38] C++：排序
来源：http://ebh.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://vyr.hongshengwenyu.top


<!-- 参考信息 -->