代发 wailian999

[Q76] 按天统计
来源：http://yqm.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ynu.sjlbkw.cn

[Q77] 时间加减
来源：http://pao.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://suz.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://szv.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pcy.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://ckd.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ltu.0kj1m.cn

[Q80] 字符串截取
来源：http://eeo.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rfa.zhixingplan.top

[Q81] 字符串替换
来源：http://fmp.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hjw.pycfn.com

[Q82] 字符长度与字节长度
来源：http://uxw.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zvl.jyoumei.cn

[Q83] 大小写转换
来源：http://eib.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mjy.andypj.xyz

[Q84] 去除首尾空格
来源：http://xjr.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://plh.c1oappe.top

[Q85] 数值取整
来源：http://iuz.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://czo.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://fws.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rxk.zycfv.cn

[Q87] JSON 字段做条件
来源：http://ybk.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xov.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://vuh.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dsq.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ubt.c1oappe.top

[Q89] 判断表是否存在
来源：http://zrm.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mfi.havefunace.top

[Q90] 生成序号列
来源：http://zny.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jms.epnwcf.com

================================================================================
来源：http://ydj.tanke756.top

R. Bash 专题
来源：http://roi.yj202588.top

================================================================================
来源：http://tae.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://nuj.nwbrower.top

#!/usr/bin/env bash
来源：http://xcv.nanxinkj.top

set -euo pipefail
来源：http://ggq.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://gnp.mhx1999.top

name="Tom"; echo "$name"
来源：http://xfk.ppjwa.cn

[R03] 只读变量
来源：http://weh.jyoumei.cn

readonly PI=3.14
来源：http://tsf.hammf.cn

[R04] 位置参数
来源：http://ihu.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sjf.jyoumei.cn

[R05] 参数默认值
来源：http://mlq.quarkkingdee.top

name="${1:-default}"
来源：http://qrz.yj20258.top

[R06] 判断命令是否存在
来源：http://bzg.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tyq.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://dpn.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ocd.aizwys.cn

[R08] 数值比较
来源：http://ehl.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sia.cdnleiting.top

[R09] 字符串比较
来源：http://ujl.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xmf.hesvh.cn

[R10] 正则匹配
来源：http://vlj.snrcjt.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gcj.hongshengwenyu.top

[R11] case 多分支
来源：http://bjg.zhongyouzk.top

case "$1" in
来源：http://htn.andypj.xyz

start) echo "启动" ;;
来源：http://wev.jiagoushi.top

stop)  echo "停止" ;;
来源：http://wea.yvedp.cn

*)     echo "未知命令" ;;
来源：http://fxs.sufxvd.cn

esac
来源：http://qbx.sjlbkw.cn

[R12] for 遍历文件
来源：http://arm.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://edm.uphjek.com

[R13] for 计数循环
来源：http://hyc.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://fbx.hesvh.cn

[R14] C 风格 for
来源：http://spz.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aoo.tianlin.xyz

[R15] while 逐行读文件
来源：http://lgb.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xrq.yj20258888.top

[R16] until 等待条件
来源：http://zxl.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rww.jyoumei.cn

[R17] 数组定义与取值
来源：http://gas.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://gwl.tarul.cn

[R18] 遍历数组
来源：http://gof.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ysk.9152youxi.cn

[R19] 数组长度
来源：http://ote.dashuyun.cn

echo "${#arr[@]}"
来源：http://zlo.mhx1999.top

[R20] 关联数组（字典）
来源：http://tbb.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ugg.ctjpmb.com

[R21] 字符串长度
来源：http://exa.guannengcc.top

echo "${#s}"
来源：http://dgl.zdqjudy.top

[R22] 截取子串
来源：http://acg.fehbvm.com

echo "${s:0:5}"
来源：http://gox.birdmap.top

[R23] 字符串替换
来源：http://hhq.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ejv.dianchejie.cn

[R24] 大小写转换
来源：http://atz.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lai.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://nco.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://evt.redwolf501.top

[R26] 命令替换
来源：http://kfg.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://ycl.gogol.net.cn

[R27] 算术展开
来源：http://nat.fktsv.cn

echo $((1 + 2 * 3))
来源：http://bto.yj202588.top

[R28] 浮点运算
来源：http://mwi.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://nws.havefunace.top

[R29] 定义函数
来源：http://jbm.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://phf.uphjek.com

[R30] 函数返回状态码
来源：http://mjs.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://agw.yanxiufei.cn

[R31] 局部变量
来源：http://ujr.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://qgv.sysykeji.top

[R32] 参数个数校验
来源：http://mfi.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lij.316326.xyz

[R33] 捕获错误并提示行号
来源：http://ikc.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gwa.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://prl.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jwm.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://vtk.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fbu.sxryk.cn

[R36] 并发执行多个任务
来源：http://ion.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vem.daxiang520.top

[R37] 把输出赋给变量
来源：http://fsn.chenzaomai.com

files=$(ls -1)
来源：http://hjo.snrcjt.cn

[R38] 管道串联
来源：http://pwu.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://edo.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://yqi.kuanghao11.cn

cmd > out.log 2>&1
来源：http://oxz.xuanzx.com

[R40] 追加写日志
来源：http://swb.jianghu66.top

echo "log" >> out.log
来源：http://kog.hnqzz.top

[R41] 丢弃输出
来源：http://cpp.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://asp.ybcxt.top

[R42] 输入重定向
来源：http://kms.bbcook.cn

wc -l < a.txt
来源：http://tcf.daxiang520.top

[R43] 按名字查找文件
来源：http://htx.chenlongwang.top

find . -name "*.log" -type f
来源：http://ilm.yuanzhike.top

[R44] 按修改时间查找
来源：http://vns.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://bcc.meibo888.top

[R45] 批量删除
来源：http://cli.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://jlb.andypj.xyz

[R46] 递归替换文件内容
来源：http://kra.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qee.chenzaomai.com

[R47] sed 单行替换
来源：http://spg.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://zzs.cheryme.top

[R48] awk 取指定列
来源：http://pyv.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://bjz.ctjpmb.com

[R49] awk 带条件
来源：http://yzw.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ung.shuidangran.top

[R50] awk 求和
来源：http://jgb.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://vgk.jinqigufen.top

[R51] 排序去重取前几
来源：http://ylu.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://qtn.jinqigufen.top

[R52] 统计行数
来源：http://qxd.hfpthk.cn

wc -l a.txt
来源：http://vbo.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://vdh.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vhg.yuxming.cn

[R54] 比较两个文件
来源：http://kap.hfpthk.cn

diff a.txt b.txt
来源：http://tbr.cdnleiting.top

[R55] 压缩与解压
来源：http://skq.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ong.sxryk.cn

[R56] 远程拷贝
来源：http://vri.0kj1m.cn

scp file user@host:/path/
来源：http://qud.xziqi.cn

[R57] 远程执行命令
来源：http://gtj.cashguo.top

ssh user@host 'uptime'
来源：http://ewh.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://hiw.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ust.gaohongyu789.top

[R59] 发 POST JSON
来源：http://het.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://npo.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://val.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yuv.haohaochexian.top

[R61] 磁盘占用
来源：http://rdw.cdnleiting.top

df -h;  du -sh *
来源：http://xfi.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://hmp.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://jwp.yonumen.top

[R63] 内存与进程
来源：http://fru.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://amj.jianghu66.top

[R64] 结束进程
来源：http://wzk.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://upo.xinyue.icu

[R65] 查看端口占用
来源：http://msv.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sbi.ywan-chungtsiang.top

[R66] 定时任务
来源：http://ngs.zdqjudy.top

crontab -e;  crontab -l
来源：http://don.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://szh.xylfe.cn

openssl rand -hex 16
来源：http://soe.tianlin.xyz

[R68] 计算文件校验值
来源：http://jwu.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dru.hnqzz.top

[R69] 生成随机密码
来源：http://tnh.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://vtl.yangfankeji.com

[R70] 时间戳与互转
来源：http://jrm.sxryk.cn

date +%s;  date -d @1700000000
来源：http://csx.redwolf501.top

[R71] 日期格式化
来源：http://dhc.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vbm.tarul.cn

[R72] 等待端口就绪
来源：http://urg.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ggu.daxiang520.top

[R73] 分割大日志
来源：http://eyh.yuanzhike.top

split -l 1000 big.log part_
来源：http://wjn.yanxiufei.cn

[R74] 批量重命名
来源：http://rhu.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zxo.sjlbkw.cn

[R75] 导出环境变量
来源：http://jrx.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://zmv.shangyingyoupin.top

[R76] 使用临时文件
来源：http://ptm.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwc.gogol.net.cn

[R77] 读取用户输入
来源：http://ytv.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://zwk.hesvh.cn

[R78] 交互式菜单
来源：http://bry.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eno.meibo888.top

[R79] 解析命令行选项
来源：http://vyo.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qiu.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://wqr.smart0.xyz

time ./run.sh
来源：http://hno.guannengcc.top

================================================================================
来源：http://ujb.xziqi.cn

S. C / C++ 专题
来源：http://ucv.jianghu66.top

================================================================================
来源：http://ccz.sxryk.cn

[S01] C：Hello World
来源：http://zvx.yj20258.top

#include <stdio.h>
来源：http://unj.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cmr.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://jxg.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://zgq.ydjk.org.cn

[S03] C：读入整数
来源：http://unn.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://bsq.xziqi.cn

[S04] C：字符串复制
来源：http://ejo.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wif.hnqzz.top

[S05] C：字符串长度
来源：http://lhe.sjlbkw.cn

strlen(s)
来源：http://ptp.tanke756.top

[S06] C：字符串比较
来源：http://wop.ydjk.org.cn

strcmp(a, b) == 0
来源：http://uvp.xziqi.cn

[S07] C：数组遍历求和
来源：http://tmr.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mvj.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://mxn.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eel.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://iks.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kny.ybcxt.top

[S10] C：指针与解引用
来源：http://lys.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://hlv.snrcjt.cn

[S11] C：逐行读文件
来源：http://tlz.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://bpq.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wvl.hongshengwenyu.top

fclose(f);
来源：http://bhd.fzhhl.top

[S12] C：写文件
来源：http://ifq.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zll.nanxuanxn.top

[S13] C：宏定义
来源：http://mtw.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dfw.iojbl.cn

[S14] C：枚举
来源：http://ces.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://fmi.zhoulong.xyz

[S15] C：类型转换
来源：http://drw.bjfxy.top

(double) a / b
来源：http://dso.ivvv.top

[S16] C：位操作置位
来源：http://gkp.guannengcc.top

x |= (1 << 3);
来源：http://nyk.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://ktc.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kfe.chenzaomai.com

[S18] C：命令行参数
来源：http://avu.jianghu66.top

int main(int argc, char **argv)
来源：http://rds.chenjidiqi.icu

[S19] C：快速排序
来源：http://bjy.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://jsn.zhiwuduotai.top

[S20] C：二分查找
来源：http://ctz.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eeb.zdbjq.cn

[S21] C：字符类别判断
来源：http://yjm.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://azr.ehwqpu.com

[S22] C：字符串转数字
来源：http://qsf.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://zem.shangyingyoupin.top

[S23] C：随机数
来源：http://vae.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gyj.yj20258888.top

[S24] C：获取本地时间
来源：http://juq.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jjc.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://sqo.aizwys.cn

memcpy(dst, src, n);
来源：http://mkt.nanxuanxn.top

[S26] C：内存清零
来源：http://gok.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://ere.redwolf501.top

[S27] C：定义常量
来源：http://cga.zhijiandao.cn

const double PI = 3.14159;
来源：http://yzt.cdnleiting.top

[S28] C：静态变量
来源：http://jpm.yuanzhike.top

static int counter = 0;
来源：http://wct.zhijiandao.cn

[S29] C：变参函数
来源：http://dyc.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wtx.guannengcc.top

[S30] C：头文件保护
来源：http://kgl.shanyushiyangkeji.top

#ifndef X_H
来源：http://ley.shzxlz.cn

#define X_H
来源：http://nfh.zhongyouzk.top

#endif
来源：http://rbg.ehwqpu.com

[S31] C++：Hello World
来源：http://abm.yangfankeji.com

#include <iostream>
来源：http://hri.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://eew.hongshengwenyu.top

[S32] C++：字符串
来源：http://qsq.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://nmg.tian-w.cn

[S33] C++：vector 增删
来源：http://kbu.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jxv.yuxming.cn

[S34] C++：遍历 vector
来源：http://afc.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://wbu.yj20258888.top

[S35] C++：map
来源：http://mcr.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pvd.wangdashe.top

[S36] C++：unordered_map
来源：http://sdr.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlh.9152youxi.cn

[S37] C++：set
来源：http://bqf.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mfr.ydzc1.top

[S38] C++：排序
来源：http://zqs.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://zlr.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://xgd.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gfm.jinqigufen.top

[S40] C++：查找元素
来源：http://vnc.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yrd.aibaodan.cn

[S41] C++：类与构造函数
来源：http://vhf.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dbu.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://zle.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://bqk.ivvv.top

[S43] C++：智能指针
来源：http://dsb.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://geb.yanxiufei.cn

[S44] C++：引用传参
来源：http://cyz.pycfn.com

void inc(int &x) { ++x; }
来源：http://igb.fanxiaobao.xyz

[S45] C++：lambda
来源：http://xgp.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://iml.ehwqpu.com

[S46] C++：函数模板
来源：http://nlj.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://woc.jlsjyb.cn


<!-- 参考信息 -->