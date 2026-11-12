代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vys.xuanzx.com

[Q75] 日期格式化
来源：http://nyw.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://muq.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ktb.9152youxi.cn

[Q76] 按天统计
来源：http://qcs.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kqf.shuidangran.top

[Q77] 时间加减
来源：http://wle.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ynj.ehwqpu.com

[Q78] 当前时间
来源：http://iek.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wrh.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://apu.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://evq.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://nll.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xjh.meibo888.top

[Q81] 字符串替换
来源：http://rpn.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zer.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://tdo.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gjg.mhx1999.top

[Q83] 大小写转换
来源：http://hau.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rlr.xinyue.icu

[Q84] 去除首尾空格
来源：http://twk.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://oml.ehwqpu.com

[Q85] 数值取整
来源：http://oby.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lek.fanxiaobao.xyz

[Q86] 读取 JSON 字段
来源：http://pxp.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vgy.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://hxn.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lkj.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://qdo.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ysm.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ejj.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://cum.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qfh.yangfankeji.com

[Q90] 生成序号列
来源：http://gkz.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jiy.yonumen.top

================================================================================
来源：http://cwy.sjlbkw.cn

R. Bash 专题
来源：http://pum.meibo888.top

================================================================================
来源：http://qkr.aizwys.cn

[R01] shebang 与严格模式
来源：http://czq.cdnleiting.top

#!/usr/bin/env bash
来源：http://ndv.gzhubu.top

set -euo pipefail
来源：http://iqc.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://mxt.fehbvm.com

name="Tom"; echo "$name"
来源：http://phy.hysaishi.cn

[R03] 只读变量
来源：http://gri.ehwqpu.com

readonly PI=3.14
来源：http://qog.yj202588.top

[R04] 位置参数
来源：http://sko.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eel.hysaishi.cn

[R05] 参数默认值
来源：http://hvm.yangfankeji.com

name="${1:-default}"
来源：http://lfh.yj20258888.top

[R06] 判断命令是否存在
来源：http://aas.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://khs.sweek.top

[R07] if 判断文件
来源：http://xsu.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://imb.aibaodan.cn

[R08] 数值比较
来源：http://iyf.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://day.gogol.net.cn

[R09] 字符串比较
来源：http://ihp.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jvk.svipenyu.cn

[R10] 正则匹配
来源：http://dox.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://olc.yongpay.top

[R11] case 多分支
来源：http://uvi.jqgfzy.top

case "$1" in
来源：http://bsq.nwbrower.top

start) echo "启动" ;;
来源：http://bom.dianchejie.cn

stop)  echo "停止" ;;
来源：http://lio.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://dku.andypj.xyz

esac
来源：http://bpg.uphjek.com

[R12] for 遍历文件
来源：http://khp.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://rze.9152youxi.cn

[R13] for 计数循环
来源：http://ady.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://onl.cdnleiting.top

[R14] C 风格 for
来源：http://ljd.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ljw.fehbvm.com

[R15] while 逐行读文件
来源：http://ouq.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hkf.52xcode.cn

[R16] until 等待条件
来源：http://tcd.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://frx.zhongyouzk.top

[R17] 数组定义与取值
来源：http://kik.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://hks.hnqzz.top

[R18] 遍历数组
来源：http://amy.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://onu.hongshengwenyu.top

[R19] 数组长度
来源：http://vgx.aibaodan.cn

echo "${#arr[@]}"
来源：http://iah.jyoumei.cn

[R20] 关联数组（字典）
来源：http://eij.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://elk.hysaishi.cn

[R21] 字符串长度
来源：http://qgi.ydjk.org.cn

echo "${#s}"
来源：http://ged.yongpay.top

[R22] 截取子串
来源：http://agd.meibo888.top

echo "${s:0:5}"
来源：http://uwq.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://wwm.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qpm.sufxvd.cn

[R24] 大小写转换
来源：http://cqv.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://spr.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://aab.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://sjr.daria6918.cn

[R26] 命令替换
来源：http://iof.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://udg.tanke756.top

[R27] 算术展开
来源：http://xaz.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://qjv.iojbl.cn

[R28] 浮点运算
来源：http://eze.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://lpq.birdmap.top

[R29] 定义函数
来源：http://auv.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://edj.andypj.xyz

[R30] 函数返回状态码
来源：http://sck.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://cmi.fktsv.cn

[R31] 局部变量
来源：http://nbh.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://wvb.meibo888.top

[R32] 参数个数校验
来源：http://ulk.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xdc.nwbrower.top

[R33] 捕获错误并提示行号
来源：http://abm.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rej.cdnleiting.top

[R34] 退出时清理
来源：http://vet.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://ste.52xcode.cn

[R35] 后台执行并等待
来源：http://xcs.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://iiv.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://kml.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yju.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://kev.fanxiaobao.xyz

files=$(ls -1)
来源：http://waz.hnxiangtu.top

[R38] 管道串联
来源：http://ssd.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://xgc.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://pto.vqdsnc.cn

cmd > out.log 2>&1
来源：http://ubj.yvedp.cn

[R40] 追加写日志
来源：http://nyq.0kj1m.cn

echo "log" >> out.log
来源：http://xcg.fktsv.cn

[R41] 丢弃输出
来源：http://jli.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://ejq.yvedp.cn

[R42] 输入重定向
来源：http://bhl.aibaodan.cn

wc -l < a.txt
来源：http://opl.zycfv.cn

[R43] 按名字查找文件
来源：http://tsr.cheryme.top

find . -name "*.log" -type f
来源：http://inm.hfpthk.cn

[R44] 按修改时间查找
来源：http://tsa.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://bgy.gogol.net.cn

[R45] 批量删除
来源：http://yua.bjfxy.top

find . -name "*.tmp" -delete
来源：http://bka.yuxming.cn

[R46] 递归替换文件内容
来源：http://uyq.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhz.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://lgc.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://urd.yangfankeji.com

[R48] awk 取指定列
来源：http://iza.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://cmi.ydzc1.top

[R49] awk 带条件
来源：http://may.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xwj.hywenlv.cn

[R50] awk 求和
来源：http://ieh.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxu.zhengqikj.top

[R51] 排序去重取前几
来源：http://wee.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ozz.sufxvd.cn

[R52] 统计行数
来源：http://dho.jinqigufen.top

wc -l a.txt
来源：http://urw.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://wmi.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uns.guannengcc.top

[R54] 比较两个文件
来源：http://dju.yanxiufei.cn

diff a.txt b.txt
来源：http://zay.nwbrower.top

[R55] 压缩与解压
来源：http://jiw.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hky.xziqi.cn

[R56] 远程拷贝
来源：http://ogt.kuanghao11.cn

scp file user@host:/path/
来源：http://dkm.wangdashe.top

[R57] 远程执行命令
来源：http://wzm.tarul.cn

ssh user@host 'uptime'
来源：http://hyc.sjlbkw.cn

[R58] 下载文件
来源：http://jfa.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ulb.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://wxi.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqq.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://jmp.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://icn.ybcxt.top

[R61] 磁盘占用
来源：http://iuf.hcnkem.com

df -h;  du -sh *
来源：http://cwf.tanke756.top

[R62] 找最占空间的文件
来源：http://bfl.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://pmp.316326.xyz

[R63] 内存与进程
来源：http://xew.cashguo.top

free -h;  ps aux | grep nginx
来源：http://bgz.yueranfly.top

[R64] 结束进程
来源：http://vqx.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://nnf.aizwys.cn

[R65] 查看端口占用
来源：http://aqy.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bpw.ehwqpu.com

[R66] 定时任务
来源：http://ftj.zhengqikj.top

crontab -e;  crontab -l
来源：http://fcp.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://azs.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://has.yvedp.cn

[R68] 计算文件校验值
来源：http://ycn.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://ibe.0kj1m.cn

[R69] 生成随机密码
来源：http://tmw.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://krz.havefunace.top

[R70] 时间戳与互转
来源：http://ipg.xinyue.icu

date +%s;  date -d @1700000000
来源：http://keo.ctjpmb.com

[R71] 日期格式化
来源：http://jsq.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://top.ybcxt.top

[R72] 等待端口就绪
来源：http://axt.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yac.smart0.xyz

[R73] 分割大日志
来源：http://dpy.guannengcc.top

split -l 1000 big.log part_
来源：http://jfk.snrcjt.cn

[R74] 批量重命名
来源：http://ivq.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eia.cqqwz.cn

[R75] 导出环境变量
来源：http://kgb.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://mnp.yonumen.top

[R76] 使用临时文件
来源：http://dbf.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dxs.ppjwa.cn

[R77] 读取用户输入
来源：http://vjh.quarkkingdee.top

read -rp "请输入: " ans
来源：http://xrk.sysykeji.top

[R78] 交互式菜单
来源：http://cti.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://deo.jlsjyb.cn

[R79] 解析命令行选项
来源：http://lpi.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gun.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://hga.yj20258888.top

time ./run.sh
来源：http://qzf.daria6918.cn

================================================================================
来源：http://ppk.smart0.xyz

S. C / C++ 专题
来源：http://bvm.0kj1m.cn

================================================================================
来源：http://gtd.kuanghao11.cn

[S01] C：Hello World
来源：http://nxy.ivvv.top

#include <stdio.h>
来源：http://ceo.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dak.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://nyg.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://xha.guowangkeji.top

[S03] C：读入整数
来源：http://pto.gotoacloud.top

int x; scanf("%d", &x);
来源：http://yvf.redwolf501.top

[S04] C：字符串复制
来源：http://xrm.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nql.chenlongwang.top

[S05] C：字符串长度
来源：http://dpa.0kj1m.cn

strlen(s)
来源：http://rel.zhoulong.xyz

[S06] C：字符串比较
来源：http://lnq.guannengcc.top

strcmp(a, b) == 0
来源：http://ftq.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://yyf.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ngx.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://qad.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uzp.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://pmq.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oqj.yonumen.top

[S10] C：指针与解引用
来源：http://jjh.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://auj.cheryme.top

[S11] C：逐行读文件
来源：http://udz.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://wdz.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ifp.daxiang520.top

fclose(f);
来源：http://xmt.gzhubu.top

[S12] C：写文件
来源：http://yoy.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wya.yangfankeji.com

[S13] C：宏定义
来源：http://dud.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ppw.cucudq.cn

[S14] C：枚举
来源：http://xry.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://riw.52xcode.cn

[S15] C：类型转换
来源：http://anp.nanxinkj.top

(double) a / b
来源：http://gca.xinyue.icu

[S16] C：位操作置位
来源：http://jta.chenjidiqi.icu

x |= (1 << 3);
来源：http://ypl.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://rdk.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fwc.vqdsnc.cn

[S18] C：命令行参数
来源：http://tyv.fzhhl.top

int main(int argc, char **argv)
来源：http://rwb.cdnleiting.top

[S19] C：快速排序
来源：http://fmb.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rou.ppjwa.cn

[S20] C：二分查找
来源：http://tdc.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sru.snrcjt.cn

[S21] C：字符类别判断
来源：http://tyv.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hek.cucudq.cn

[S22] C：字符串转数字
来源：http://uui.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cac.wangdashe.top

[S23] C：随机数
来源：http://nyg.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://xsu.fzhhl.top

[S24] C：获取本地时间
来源：http://mex.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hcr.ydzc1.top

[S25] C：内存拷贝
来源：http://cbn.andypj.xyz

memcpy(dst, src, n);
来源：http://phf.xinyue.icu

[S26] C：内存清零
来源：http://iyz.tanke756.top

memset(a, 0, sizeof a);
来源：http://qfo.sweek.top

[S27] C：定义常量
来源：http://jxl.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://mbo.hesvh.cn

[S28] C：静态变量
来源：http://wuf.guowangkeji.top

static int counter = 0;
来源：http://tcu.xuanzx.com

[S29] C：变参函数
来源：http://fhq.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etv.zhixingplan.top

[S30] C：头文件保护
来源：http://kwi.sjlbkw.cn

#ifndef X_H
来源：http://lge.shzxlz.cn

#define X_H
来源：http://jfs.vqdsnc.cn

#endif
来源：http://utq.cheryme.top

[S31] C++：Hello World
来源：http://pqo.meibo888.top

#include <iostream>
来源：http://byd.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://xje.cdnleiting.top

[S32] C++：字符串
来源：http://lli.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://xoh.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://ydu.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eew.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://sab.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://qjx.feifeiyinyue.top

[S35] C++：map
来源：http://inv.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vuq.xziqi.cn

[S36] C++：unordered_map
来源：http://ajk.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rtt.chenzaomai.com

[S37] C++：set
来源：http://cwd.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bha.pengpengdd.cyou

[S38] C++：排序
来源：http://kbs.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://dqq.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://qkz.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://glw.nwbrower.top

[S40] C++：查找元素
来源：http://vql.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fis.fzhhl.top

[S41] C++：类与构造函数
来源：http://jfr.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://thf.aizwys.cn

[S42] C++：继承与虚函数
来源：http://etk.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://auf.nanxinkj.top

[S43] C++：智能指针
来源：http://ner.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://sym.ydjk.org.cn

[S44] C++：引用传参
来源：http://jni.fehbvm.com

void inc(int &x) { ++x; }
来源：http://xex.gogol.net.cn


<!-- 参考信息 -->