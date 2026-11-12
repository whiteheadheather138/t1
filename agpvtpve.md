代发 wailian999

[Q76] 按天统计
来源：http://ohz.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mrv.yanxiufei.cn

[Q77] 时间加减
来源：http://rar.tarul.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://swi.ppjwa.cn

[Q78] 当前时间
来源：http://zrb.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vcq.xziqi.cn

[Q79] 字符串拼接
来源：http://alj.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cpi.jinqigufen.top

[Q80] 字符串截取
来源：http://jky.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wvy.svipenyu.cn

[Q81] 字符串替换
来源：http://jjx.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jwp.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://dmr.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bcl.yj20258.top

[Q83] 大小写转换
来源：http://hbn.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kyy.ctjpmb.com

[Q84] 去除首尾空格
来源：http://jaq.redwolf501.top

SELECT TRIM(name) FROM users;
来源：http://uwi.svipenyu.cn

[Q85] 数值取整
来源：http://zgo.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jtf.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://prf.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://trp.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://rwo.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rgj.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://cim.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lwq.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oxm.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://cgm.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gbz.yuanzhike.top

[Q90] 生成序号列
来源：http://ujw.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://unc.aizwys.cn

================================================================================
来源：http://yce.zycfv.cn

R. Bash 专题
来源：http://qcf.fktsv.cn

================================================================================
来源：http://qzx.gzhubu.top

[R01] shebang 与严格模式
来源：http://tzq.jinqigufen.top

#!/usr/bin/env bash
来源：http://gpc.zhijiandao.cn

set -euo pipefail
来源：http://ygs.mhx1999.top

[R02] 变量赋值与使用
来源：http://ffs.xuanzx.com

name="Tom"; echo "$name"
来源：http://uro.shzxlz.cn

[R03] 只读变量
来源：http://wwe.zhijiandao.cn

readonly PI=3.14
来源：http://trz.shuidangran.top

[R04] 位置参数
来源：http://ise.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rhv.guowangkeji.top

[R05] 参数默认值
来源：http://nho.xylfe.cn

name="${1:-default}"
来源：http://npk.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://mkm.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fvx.aizwys.cn

[R07] if 判断文件
来源：http://gyf.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://are.zhongyouzk.top

[R08] 数值比较
来源：http://gbc.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cqh.ctjpmb.com

[R09] 字符串比较
来源：http://mqz.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yjn.zycfv.cn

[R10] 正则匹配
来源：http://ksa.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gqk.hysaishi.cn

[R11] case 多分支
来源：http://uib.nanxuanxn.top

case "$1" in
来源：http://meq.vqdsnc.cn

start) echo "启动" ;;
来源：http://wec.daxiang520.top

stop)  echo "停止" ;;
来源：http://waa.52xcode.cn

*)     echo "未知命令" ;;
来源：http://tqm.zhongyouzk.top

esac
来源：http://dbl.hammf.cn

[R12] for 遍历文件
来源：http://diw.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://cwc.yj20258.top

[R13] for 计数循环
来源：http://tzm.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://asg.tarul.cn

[R14] C 风格 for
来源：http://ulg.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gtg.xuanzx.com

[R15] while 逐行读文件
来源：http://tgr.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://esg.yj202588.top

[R16] until 等待条件
来源：http://ieq.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jps.jqgfzy.top

[R17] 数组定义与取值
来源：http://vuy.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://xif.gotoacloud.top

[R18] 遍历数组
来源：http://mos.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zaf.dashuyun.cn

[R19] 数组长度
来源：http://sii.hcnkem.com

echo "${#arr[@]}"
来源：http://bxi.cdnleiting.top

[R20] 关联数组（字典）
来源：http://qkp.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://llc.yongpay.top

[R21] 字符串长度
来源：http://fex.zhengqikj.top

echo "${#s}"
来源：http://yod.zhixingplan.top

[R22] 截取子串
来源：http://skv.52xcode.cn

echo "${s:0:5}"
来源：http://ctw.feifeiyinyue.top

[R23] 字符串替换
来源：http://vui.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uyc.chenlongwang.top

[R24] 大小写转换
来源：http://tml.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wtm.jqgfzy.top

[R25] 去后缀 / 去前缀
来源：http://exx.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://euq.tianlin.xyz

[R26] 命令替换
来源：http://nam.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://adn.yuanzhike.top

[R27] 算术展开
来源：http://muw.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://fqo.shuidangran.top

[R28] 浮点运算
来源：http://ngs.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://xqg.0kj1m.cn

[R29] 定义函数
来源：http://wpm.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vnt.jqgfzy.top

[R30] 函数返回状态码
来源：http://jvl.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://win.sjlbkw.cn

[R31] 局部变量
来源：http://ovm.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://nem.zhijiandao.cn

[R32] 参数个数校验
来源：http://wmr.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oml.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://tgf.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xee.shanyushiyangtech.top

[R34] 退出时清理
来源：http://ayd.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jxf.jqgufenzy.top

[R35] 后台执行并等待
来源：http://ysy.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://opc.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://wmd.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dve.aizwys.cn

[R37] 把输出赋给变量
来源：http://gof.iojbl.cn

files=$(ls -1)
来源：http://sxv.chenjidiqi.icu

[R38] 管道串联
来源：http://zej.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://dls.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://fgn.52xcode.cn

cmd > out.log 2>&1
来源：http://fml.sufxvd.cn

[R40] 追加写日志
来源：http://hhv.bjfxy.top

echo "log" >> out.log
来源：http://fqf.uphjek.com

[R41] 丢弃输出
来源：http://zwn.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://otg.tarul.cn

[R42] 输入重定向
来源：http://kfn.redwolf501.top

wc -l < a.txt
来源：http://kym.jianghu66.top

[R43] 按名字查找文件
来源：http://ios.hfpthk.cn

find . -name "*.log" -type f
来源：http://ggn.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://oyt.nanxinkj.top

find . -mtime -7 -type f
来源：http://kcd.aibaodan.cn

[R45] 批量删除
来源：http://eqh.tian-w.cn

find . -name "*.tmp" -delete
来源：http://kgg.hfpthk.cn

[R46] 递归替换文件内容
来源：http://ydh.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sky.gogol.net.cn

[R47] sed 单行替换
来源：http://tav.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://uuo.fktsv.cn

[R48] awk 取指定列
来源：http://eat.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://qod.xziqi.cn

[R49] awk 带条件
来源：http://zyz.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ekp.jinqigfzy.top

[R50] awk 求和
来源：http://aya.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://aoe.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://xuc.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vhu.guannengcc.top

[R52] 统计行数
来源：http://zgg.xylfe.cn

wc -l a.txt
来源：http://siv.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://ptr.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://chx.yongpay.top

[R54] 比较两个文件
来源：http://ilx.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://fsl.yj20258.top

[R55] 压缩与解压
来源：http://yga.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sue.hywenlv.cn

[R56] 远程拷贝
来源：http://rgp.mhx1999.top

scp file user@host:/path/
来源：http://uiw.haohaochexian.top

[R57] 远程执行命令
来源：http://owe.zhongyouzk.top

ssh user@host 'uptime'
来源：http://ztm.yvedp.cn

[R58] 下载文件
来源：http://skd.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qoo.gogol.net.cn

[R59] 发 POST JSON
来源：http://bsq.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ujz.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://pch.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zzy.feifeiyinyue.top

[R61] 磁盘占用
来源：http://eny.wangdashe.top

df -h;  du -sh *
来源：http://ksf.zhengqikj.top

[R62] 找最占空间的文件
来源：http://ygt.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://kfp.gotoacloud.top

[R63] 内存与进程
来源：http://iyg.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://dtj.yj20258888.top

[R64] 结束进程
来源：http://lde.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://xda.ctjpmb.com

[R65] 查看端口占用
来源：http://toh.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bgt.redwolf501.top

[R66] 定时任务
来源：http://xcl.yonumen.top

crontab -e;  crontab -l
来源：http://bzv.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://mee.sufxvd.cn

openssl rand -hex 16
来源：http://dmv.wangdashe.top

[R68] 计算文件校验值
来源：http://wgn.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://nqt.birdmap.top

[R69] 生成随机密码
来源：http://qtf.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://yez.tarul.cn

[R70] 时间戳与互转
来源：http://usz.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://nsb.snrcjt.cn

[R71] 日期格式化
来源：http://goc.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bsd.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://meq.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zjy.guannengcc.top

[R73] 分割大日志
来源：http://phn.birdmap.top

split -l 1000 big.log part_
来源：http://gqq.sxryk.cn

[R74] 批量重命名
来源：http://hra.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qhx.ivvv.top

[R75] 导出环境变量
来源：http://yse.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://nbz.svipenyu.cn

[R76] 使用临时文件
来源：http://zvl.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://znx.nwbrower.top

[R77] 读取用户输入
来源：http://itr.gaohongyu789.top

read -rp "请输入: " ans
来源：http://zgq.nanxuanxn.top

[R78] 交互式菜单
来源：http://uok.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uvt.gaohongyu789.top

[R79] 解析命令行选项
来源：http://awm.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jpf.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://mao.jyoumei.cn

time ./run.sh
来源：http://ihq.yangfankeji.com

================================================================================
来源：http://kwe.gaohongyu789.top

S. C / C++ 专题
来源：http://otx.jqgufenzy.top

================================================================================
来源：http://ria.redwolf501.top

[S01] C：Hello World
来源：http://ppw.hesvh.cn

#include <stdio.h>
来源：http://tvj.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://zyr.yuxming.cn

[S02] C：变量与格式化输出
来源：http://jcr.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://cmn.sufxvd.cn

[S03] C：读入整数
来源：http://rwo.tianlin.xyz

int x; scanf("%d", &x);
来源：http://fzp.tarul.cn

[S04] C：字符串复制
来源：http://zsw.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uct.yvedp.cn

[S05] C：字符串长度
来源：http://iog.316326.xyz

strlen(s)
来源：http://qiq.mhx1999.top

[S06] C：字符串比较
来源：http://ojc.guowangkeji.top

strcmp(a, b) == 0
来源：http://lro.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://lde.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qdt.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://jzu.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bub.birdmap.top

[S09] C：结构体定义与初始化
来源：http://jpz.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ycr.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://swl.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://qoy.snrcjt.cn

[S11] C：逐行读文件
来源：http://acz.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://omt.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zxk.ivvv.top

fclose(f);
来源：http://jnh.wangshuangyany.cn

[S12] C：写文件
来源：http://pyv.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ukd.hywenlv.cn

[S13] C：宏定义
来源：http://nsm.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qgs.aibaodan.cn

[S14] C：枚举
来源：http://bxv.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://cqk.gzhubu.top

[S15] C：类型转换
来源：http://xyd.vqdsnc.cn

(double) a / b
来源：http://sil.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://hyx.smart0.xyz

x |= (1 << 3);
来源：http://srz.daria6918.cn

[S17] C：安全拼接字符串
来源：http://kdp.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pqf.ctjpmb.com

[S18] C：命令行参数
来源：http://vfh.nanxinkj.top

int main(int argc, char **argv)
来源：http://cvh.svipenyu.cn

[S19] C：快速排序
来源：http://bwl.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://tdg.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://ouh.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bcj.hysaishi.cn

[S21] C：字符类别判断
来源：http://qua.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfq.andypj.xyz

[S22] C：字符串转数字
来源：http://jff.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://wjd.jinqigufen.top

[S23] C：随机数
来源：http://zed.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bhi.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://tov.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xtv.epnwcf.com

[S25] C：内存拷贝
来源：http://gru.xinyue.icu

memcpy(dst, src, n);
来源：http://jom.fktsv.cn

[S26] C：内存清零
来源：http://oxp.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://ofd.jinqigufen.top

[S27] C：定义常量
来源：http://ptk.jlsjyb.cn

const double PI = 3.14159;
来源：http://mmt.cdnleiting.top

[S28] C：静态变量
来源：http://pfa.yueranfly.top

static int counter = 0;
来源：http://tbv.cqqwz.cn

[S29] C：变参函数
来源：http://rim.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://glk.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://pjk.shanyushiyangtech.top

#ifndef X_H
来源：http://ajy.smart0.xyz

#define X_H
来源：http://ktx.316326.xyz

#endif
来源：http://ejq.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://ggd.xingfuxueyuan.xyz

#include <iostream>
来源：http://rzg.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://nkh.fktsv.cn

[S32] C++：字符串
来源：http://qui.yj20258.top

std::string s = "hi";  s += "!";
来源：http://ukj.vqdsnc.cn

[S33] C++：vector 增删
来源：http://jpk.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dsa.ydzc1.top

[S34] C++：遍历 vector
来源：http://qrr.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://fld.chenjidiqi.icu

[S35] C++：map
来源：http://faz.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qjc.chenzaomai.com

[S36] C++：unordered_map
来源：http://fok.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xrq.jqgufenzy.top

[S37] C++：set
来源：http://tnl.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zyr.hcnkem.com

[S38] C++：排序
来源：http://mug.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://nez.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://qdm.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://unb.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://for.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sml.ydzc1.top

[S41] C++：类与构造函数
来源：http://dpe.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xnu.ydzc1.top

[S42] C++：继承与虚函数
来源：http://gdq.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://vqd.dianchejie.cn

[S43] C++：智能指针
来源：http://gbn.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://uwz.chenzaomai.com

[S44] C++：引用传参
来源：http://bhw.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://dpf.gzhubu.top

[S45] C++：lambda
来源：http://hgg.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://zwj.yfazqb.com

[S46] C++：函数模板
来源：http://woa.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://smt.chenjidiqi.icu


<!-- 参考信息 -->