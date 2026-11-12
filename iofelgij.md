代发 wailian999

[Q76] 按天统计
来源：http://gej.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://txf.tian-w.cn

[Q77] 时间加减
来源：http://ghe.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://suy.ehwqpu.com

[Q78] 当前时间
来源：http://xod.316326.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rbc.chenzaomai.com

[Q79] 字符串拼接
来源：http://luy.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zfp.ppjwa.cn

[Q80] 字符串截取
来源：http://kvn.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vmz.gzhubu.top

[Q81] 字符串替换
来源：http://syj.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://idc.cashguo.top

[Q82] 字符长度与字节长度
来源：http://eoa.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fpk.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://egp.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wmr.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://qwx.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://fkk.hfpthk.cn

[Q85] 数值取整
来源：http://aqo.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eur.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://rbr.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nqr.shanyushiyangkeji.top

[Q87] JSON 字段做条件
来源：http://wbp.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://acp.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://tca.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yhl.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kzy.dianchejie.cn

[Q89] 判断表是否存在
来源：http://dki.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fij.zhijiandao.cn

[Q90] 生成序号列
来源：http://jil.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uez.zdbjq.cn

================================================================================
来源：http://fyg.dianchejie.cn

R. Bash 专题
来源：http://apu.yj20258.top

================================================================================
来源：http://mlo.52xcode.cn

[R01] shebang 与严格模式
来源：http://zai.xylfe.cn

#!/usr/bin/env bash
来源：http://lmc.yongpay.top

set -euo pipefail
来源：http://zhq.ydzc1.top

[R02] 变量赋值与使用
来源：http://gpa.ivvv.top

name="Tom"; echo "$name"
来源：http://fgy.jiagoushi.top

[R03] 只读变量
来源：http://uxz.hesvh.cn

readonly PI=3.14
来源：http://jez.ybcxt.top

[R04] 位置参数
来源：http://gjh.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lpf.sxryk.cn

[R05] 参数默认值
来源：http://nel.yvedp.cn

name="${1:-default}"
来源：http://bdc.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://mxh.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bvk.yuxming.cn

[R07] if 判断文件
来源：http://fbj.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vma.ctjpmb.com

[R08] 数值比较
来源：http://gkg.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://axx.shzxlz.cn

[R09] 字符串比较
来源：http://jno.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bpg.sweek.top

[R10] 正则匹配
来源：http://jhm.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zfb.shanyushiyangtech.top

[R11] case 多分支
来源：http://sal.0kj1m.cn

case "$1" in
来源：http://ltw.gzhubu.top

start) echo "启动" ;;
来源：http://gvv.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://mib.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://sxm.fengsongda.top

esac
来源：http://nsq.zhijiandao.cn

[R12] for 遍历文件
来源：http://jun.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://feh.hongshengwenyu.top

[R13] for 计数循环
来源：http://iwg.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://gyy.gaohongyu789.top

[R14] C 风格 for
来源：http://aae.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://umm.yfazqb.com

[R15] while 逐行读文件
来源：http://ozt.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rlm.vqdsnc.cn

[R16] until 等待条件
来源：http://xpj.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ehp.kuanghao11.cn

[R17] 数组定义与取值
来源：http://qyz.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://qay.chenzaomai.com

[R18] 遍历数组
来源：http://oad.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://awu.xziqi.cn

[R19] 数组长度
来源：http://oux.jqgfzy.top

echo "${#arr[@]}"
来源：http://keh.yj20258.top

[R20] 关联数组（字典）
来源：http://jjm.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ums.zhengqikj.top

[R21] 字符串长度
来源：http://oho.hywenlv.cn

echo "${#s}"
来源：http://wcl.xuanzx.com

[R22] 截取子串
来源：http://yos.yfazqb.com

echo "${s:0:5}"
来源：http://cel.jinghuilouyu.cn

[R23] 字符串替换
来源：http://yqw.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gxd.yueranfly.top

[R24] 大小写转换
来源：http://oii.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://mly.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://zyx.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kir.gotoacloud.top

[R26] 命令替换
来源：http://mdu.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://iqa.redwolf501.top

[R27] 算术展开
来源：http://fiw.bbcook.cn

echo $((1 + 2 * 3))
来源：http://tkq.mhx1999.top

[R28] 浮点运算
来源：http://lku.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://uho.yuxming.cn

[R29] 定义函数
来源：http://mpp.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fqb.daria6918.cn

[R30] 函数返回状态码
来源：http://wqd.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://wfc.mhx1999.top

[R31] 局部变量
来源：http://zrl.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://yyq.xinyue.icu

[R32] 参数个数校验
来源：http://chs.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ssp.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://heh.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://doz.0kj1m.cn

[R34] 退出时清理
来源：http://jnx.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://cuf.andypj.xyz

[R35] 后台执行并等待
来源：http://qbn.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gks.nwbrower.top

[R36] 并发执行多个任务
来源：http://hbi.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kns.andypj.xyz

[R37] 把输出赋给变量
来源：http://wpg.jinqigfzy.top

files=$(ls -1)
来源：http://doa.ydjk.org.cn

[R38] 管道串联
来源：http://wlh.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://wha.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://lqp.zhengqikj.top

cmd > out.log 2>&1
来源：http://sec.aizwys.cn

[R40] 追加写日志
来源：http://hwx.mhx1999.top

echo "log" >> out.log
来源：http://djt.jyoumei.cn

[R41] 丢弃输出
来源：http://nin.fzhhl.top

cmd >/dev/null 2>&1
来源：http://aoa.hesvh.cn

[R42] 输入重定向
来源：http://zqq.ybcxt.top

wc -l < a.txt
来源：http://myo.xziqi.cn

[R43] 按名字查找文件
来源：http://uds.hnqzz.top

find . -name "*.log" -type f
来源：http://hsd.jinqigufen.top

[R44] 按修改时间查找
来源：http://imp.zdbjq.cn

find . -mtime -7 -type f
来源：http://pog.wangdashe.top

[R45] 批量删除
来源：http://noq.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://ysc.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://jnx.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fwt.dashuyun.cn

[R47] sed 单行替换
来源：http://ari.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gru.yfazqb.com

[R48] awk 取指定列
来源：http://nsc.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://bkx.sysykeji.top

[R49] awk 带条件
来源：http://uke.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oys.jyoumei.cn

[R50] awk 求和
来源：http://spm.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://pcz.pycfn.com

[R51] 排序去重取前几
来源：http://jed.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://koa.ydjk.org.cn

[R52] 统计行数
来源：http://qms.daxiang520.top

wc -l a.txt
来源：http://sad.cheryme.top

[R53] 查看文件头与实时尾
来源：http://dim.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://heg.vqdsnc.cn

[R54] 比较两个文件
来源：http://uul.ppjwa.cn

diff a.txt b.txt
来源：http://ffq.vqdsnc.cn

[R55] 压缩与解压
来源：http://vfc.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zzu.chenlongwang.top

[R56] 远程拷贝
来源：http://xsb.ydjk.org.cn

scp file user@host:/path/
来源：http://fis.yonumen.top

[R57] 远程执行命令
来源：http://myc.yangfankeji.com

ssh user@host 'uptime'
来源：http://ovt.yuxming.cn

[R58] 下载文件
来源：http://vlh.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rxy.yangfankeji.com

[R59] 发 POST JSON
来源：http://yme.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xgq.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://zer.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lap.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://jjw.sweek.top

df -h;  du -sh *
来源：http://qrc.jianghu66.top

[R62] 找最占空间的文件
来源：http://qgs.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://pau.daxiang520.top

[R63] 内存与进程
来源：http://wnn.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://wxi.hywenlv.cn

[R64] 结束进程
来源：http://xlz.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://kvu.haohaochexian.top

[R65] 查看端口占用
来源：http://lnc.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fmd.haohaochexian.top

[R66] 定时任务
来源：http://tws.redwolf501.top

crontab -e;  crontab -l
来源：http://hgv.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://pop.dianchejie.cn

openssl rand -hex 16
来源：http://gnw.52xcode.cn

[R68] 计算文件校验值
来源：http://wyq.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://wvj.yuxming.cn

[R69] 生成随机密码
来源：http://fft.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://rgx.gotoacloud.top

[R70] 时间戳与互转
来源：http://msz.vehdjk.com

date +%s;  date -d @1700000000
来源：http://gol.jinqigufen.top

[R71] 日期格式化
来源：http://czg.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://obi.ivvv.top

[R72] 等待端口就绪
来源：http://rrd.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://trp.vehdjk.com

[R73] 分割大日志
来源：http://rvf.jianghu66.top

split -l 1000 big.log part_
来源：http://kqa.xuanzx.com

[R74] 批量重命名
来源：http://rqs.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ayy.zhoulong.xyz

[R75] 导出环境变量
来源：http://sss.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://bzx.cashguo.top

[R76] 使用临时文件
来源：http://oqu.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vph.hammf.cn

[R77] 读取用户输入
来源：http://sve.birdmap.top

read -rp "请输入: " ans
来源：http://dxl.yj202588.top

[R78] 交互式菜单
来源：http://rii.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ipl.shzxlz.cn

[R79] 解析命令行选项
来源：http://xbw.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fgk.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://njs.ivvv.top

time ./run.sh
来源：http://fzp.bjfxy.top

================================================================================
来源：http://fde.zhixingplan.top

S. C / C++ 专题
来源：http://fgy.jyoumei.cn

================================================================================
来源：http://jiw.birdmap.top

[S01] C：Hello World
来源：http://efa.gotoacloud.top

#include <stdio.h>
来源：http://qds.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wmr.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://cfm.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://ris.tanke756.top

[S03] C：读入整数
来源：http://elo.hnqzz.top

int x; scanf("%d", &x);
来源：http://xgs.cqqwz.cn

[S04] C：字符串复制
来源：http://vtr.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://xnl.feifeiyinyue.top

[S05] C：字符串长度
来源：http://gzs.hongshengwenyu.top

strlen(s)
来源：http://odb.hammf.cn

[S06] C：字符串比较
来源：http://xto.guannengcc.top

strcmp(a, b) == 0
来源：http://wnl.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://cxd.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aht.uphjek.com

[S08] C：动态内存分配与释放
来源：http://gbf.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yby.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://voa.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzc.meibo888.top

[S10] C：指针与解引用
来源：http://zvf.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://znw.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://slg.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://qrw.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mvb.zycfv.cn

fclose(f);
来源：http://lfr.xziqi.cn

[S12] C：写文件
来源：http://bxt.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://swu.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://vrx.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jvv.nanxuanxn.top

[S14] C：枚举
来源：http://ygb.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://jpb.snrcjt.cn

[S15] C：类型转换
来源：http://lls.aibaodan.cn

(double) a / b
来源：http://rix.hnqzz.top

[S16] C：位操作置位
来源：http://ysp.xuetiantiany.cn

x |= (1 << 3);
来源：http://laj.c1oappe.top

[S17] C：安全拼接字符串
来源：http://xwz.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zbu.daxiang520.top

[S18] C：命令行参数
来源：http://mng.hesvh.cn

int main(int argc, char **argv)
来源：http://xtb.jianghu66.top

[S19] C：快速排序
来源：http://ngy.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://jfm.ydjk.org.cn

[S20] C：二分查找
来源：http://pxz.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ims.hysaishi.cn

[S21] C：字符类别判断
来源：http://mpf.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yqk.chenzaomai.com

[S22] C：字符串转数字
来源：http://nlz.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qah.sufxvd.cn

[S23] C：随机数
来源：http://bbv.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qsv.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://uyp.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kgg.yuxming.cn

[S25] C：内存拷贝
来源：http://qww.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://hky.hywenlv.cn

[S26] C：内存清零
来源：http://vft.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://swj.yfazqb.com

[S27] C：定义常量
来源：http://amo.snrcjt.cn

const double PI = 3.14159;
来源：http://uop.jinqigfzy.top

[S28] C：静态变量
来源：http://owh.wangshuangyany.cn

static int counter = 0;
来源：http://yti.yuanzhike.top

[S29] C：变参函数
来源：http://fji.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qrn.hesvh.cn

[S30] C：头文件保护
来源：http://rox.zhongyouzk.top

#ifndef X_H
来源：http://hki.hfpthk.cn

#define X_H
来源：http://zlh.zhoulong.xyz

#endif
来源：http://sja.wangshuangyany.cn

[S31] C++：Hello World
来源：http://xmc.quarkkingdee.top

#include <iostream>
来源：http://fvk.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://xih.cqqwz.cn

[S32] C++：字符串
来源：http://qyl.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://ziv.zhixingplan.top

[S33] C++：vector 增删
来源：http://ykk.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zcm.svipenyu.cn

[S34] C++：遍历 vector
来源：http://fbp.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://jph.zhoulong.xyz

[S35] C++：map
来源：http://keq.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gbc.ydjk.org.cn

[S36] C++：unordered_map
来源：http://vsw.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nge.kuanghao11.cn

[S37] C++：set
来源：http://ufi.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wef.feifeiyinyue.top

[S38] C++：排序
来源：http://llo.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://nvs.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://sja.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mlx.xylfe.cn

[S40] C++：查找元素
来源：http://ubf.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mpa.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://pue.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qva.fehbvm.com

[S42] C++：继承与虚函数
来源：http://xbo.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://uyo.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://faw.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://fbf.nanxuanxn.top

[S44] C++：引用传参
来源：http://vwc.fengsongda.top

void inc(int &x) { ++x; }
来源：http://mxw.shzxlz.cn

[S45] C++：lambda
来源：http://hfu.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fmr.daxiang520.top

[S46] C++：函数模板
来源：http://ryp.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bqf.jiagoushi.top


<!-- 参考信息 -->