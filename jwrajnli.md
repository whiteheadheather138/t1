代发 wailian999

SHOW INDEX FROM users;
来源：http://wtz.daxiang520.top

[Q73] 查看表状态
来源：http://uma.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://awh.xziqi.cn

[Q74] 强制使用索引
来源：http://jjz.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lok.0kj1m.cn

[Q75] 日期格式化
来源：http://clm.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nxp.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lto.bjfxy.top

[Q76] 按天统计
来源：http://dgl.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xvc.wangdashe.top

[Q77] 时间加减
来源：http://lpq.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://csq.hnqzz.top

[Q78] 当前时间
来源：http://cea.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nwn.ydzc1.top

[Q79] 字符串拼接
来源：http://ton.xylfe.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ucx.nanxuanxn.top

[Q80] 字符串截取
来源：http://wkd.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uml.hongshengwenyu.top

[Q81] 字符串替换
来源：http://umy.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://szu.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://bai.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mhx.yuanzhike.top

[Q83] 大小写转换
来源：http://wxc.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hgy.aibaodan.cn

[Q84] 去除首尾空格
来源：http://kks.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://vju.havefunace.top

[Q85] 数值取整
来源：http://guj.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xxx.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://csp.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://roh.yongpay.top

[Q87] JSON 字段做条件
来源：http://oih.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bdg.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://cuu.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cbu.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://evy.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://cxi.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xhn.tianlin.xyz

[Q90] 生成序号列
来源：http://hik.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yrt.zhiwuduotai.top

================================================================================
来源：http://xmf.guannengcc.top

R. Bash 专题
来源：http://dzm.wangshuangyany.cn

================================================================================
来源：http://aju.gotoacloud.top

[R01] shebang 与严格模式
来源：http://hsl.wangdashe.top

#!/usr/bin/env bash
来源：http://roj.aizwys.cn

set -euo pipefail
来源：http://nbl.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://fex.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://ajz.zdqjudy.top

[R03] 只读变量
来源：http://eea.xinyue.icu

readonly PI=3.14
来源：http://mgw.hammf.cn

[R04] 位置参数
来源：http://elk.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lfp.chenlongwang.top

[R05] 参数默认值
来源：http://jmt.wangdashe.top

name="${1:-default}"
来源：http://tft.mhx1999.top

[R06] 判断命令是否存在
来源：http://whd.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uoy.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://zjs.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xqf.snrcjt.cn

[R08] 数值比较
来源：http://azq.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://any.jianghu66.top

[R09] 字符串比较
来源：http://gym.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ywq.guannengcc.top

[R10] 正则匹配
来源：http://xpl.daria6918.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dgk.ywan-chungtsiang.top

[R11] case 多分支
来源：http://pou.jianghu66.top

case "$1" in
来源：http://tqb.zhoulong.xyz

start) echo "启动" ;;
来源：http://yfy.sweek.top

stop)  echo "停止" ;;
来源：http://fev.aizwys.cn

*)     echo "未知命令" ;;
来源：http://onc.hnxiangtu.top

esac
来源：http://jnx.zhoulong.xyz

[R12] for 遍历文件
来源：http://yrr.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://hoj.52xcode.cn

[R13] for 计数循环
来源：http://tok.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://mrr.nanxuanxn.top

[R14] C 风格 for
来源：http://tij.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qkh.hfpthk.cn

[R15] while 逐行读文件
来源：http://tox.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ryb.aibaodan.cn

[R16] until 等待条件
来源：http://ubh.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rcu.cucudq.cn

[R17] 数组定义与取值
来源：http://bff.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://lsq.yj20258888.top

[R18] 遍历数组
来源：http://mje.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxc.yongpay.top

[R19] 数组长度
来源：http://mab.haohaochexian.top

echo "${#arr[@]}"
来源：http://wwh.gzhubu.top

[R20] 关联数组（字典）
来源：http://erx.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ddr.aibaodan.cn

[R21] 字符串长度
来源：http://dnl.aibaodan.cn

echo "${#s}"
来源：http://yvx.zhiwuduotai.top

[R22] 截取子串
来源：http://fwk.jinqigufen.top

echo "${s:0:5}"
来源：http://qna.epnwcf.com

[R23] 字符串替换
来源：http://nhs.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://okv.yj202588.top

[R24] 大小写转换
来源：http://kkq.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://fya.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://lje.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sbg.sjlbkw.cn

[R26] 命令替换
来源：http://xba.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://edw.sxryk.cn

[R27] 算术展开
来源：http://hth.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://syv.daria6918.cn

[R28] 浮点运算
来源：http://fzg.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://cfw.iojbl.cn

[R29] 定义函数
来源：http://jmh.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aqq.yanxiufei.cn

[R30] 函数返回状态码
来源：http://rxp.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://rzk.hnqzz.top

[R31] 局部变量
来源：http://eti.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://owc.gzhubu.top

[R32] 参数个数校验
来源：http://tdg.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ivh.yj202588.top

[R33] 捕获错误并提示行号
来源：http://sak.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zfw.nwbrower.top

[R34] 退出时清理
来源：http://dgc.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://oko.gogol.net.cn

[R35] 后台执行并等待
来源：http://mjw.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ydo.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://iwv.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://raf.hysaishi.cn

[R37] 把输出赋给变量
来源：http://zqo.cashguo.top

files=$(ls -1)
来源：http://xbh.ywan-chungtsiang.top

[R38] 管道串联
来源：http://cqu.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://rba.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://pxu.jiagoushi.top

cmd > out.log 2>&1
来源：http://dos.sufxvd.cn

[R40] 追加写日志
来源：http://aga.wangdashe.top

echo "log" >> out.log
来源：http://owx.fengsongda.top

[R41] 丢弃输出
来源：http://nnu.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://ngw.zhengqikj.top

[R42] 输入重定向
来源：http://boz.daxiang520.top

wc -l < a.txt
来源：http://dvu.ctjpmb.com

[R43] 按名字查找文件
来源：http://ife.gogol.net.cn

find . -name "*.log" -type f
来源：http://lgg.tanke756.top

[R44] 按修改时间查找
来源：http://ugx.tanke756.top

find . -mtime -7 -type f
来源：http://okk.jinqigufen.top

[R45] 批量删除
来源：http://kut.andypj.xyz

find . -name "*.tmp" -delete
来源：http://lrk.andypj.xyz

[R46] 递归替换文件内容
来源：http://nea.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cuu.yuanzhike.top

[R47] sed 单行替换
来源：http://weq.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://bpj.ivvv.top

[R48] awk 取指定列
来源：http://iuf.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://oay.jianghu66.top

[R49] awk 带条件
来源：http://uzg.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://frg.haohaochexian.top

[R50] awk 求和
来源：http://ssd.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://sth.sjlbkw.cn

[R51] 排序去重取前几
来源：http://bcg.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://syf.hcnkem.com

[R52] 统计行数
来源：http://baw.yj202588.top

wc -l a.txt
来源：http://hfj.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://uia.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yhk.cashguo.top

[R54] 比较两个文件
来源：http://cpd.wangshuangyany.cn

diff a.txt b.txt
来源：http://yqj.havefunace.top

[R55] 压缩与解压
来源：http://jlc.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vvs.cashguo.top

[R56] 远程拷贝
来源：http://lgy.zdqjudy.top

scp file user@host:/path/
来源：http://aaw.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://rza.tian-w.cn

ssh user@host 'uptime'
来源：http://pbq.fengsongda.top

[R58] 下载文件
来源：http://uiv.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aol.ybcxt.top

[R59] 发 POST JSON
来源：http://afi.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jqu.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://hdz.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://shl.cucudq.cn

[R61] 磁盘占用
来源：http://fmf.nanxinkj.top

df -h;  du -sh *
来源：http://puv.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://zfx.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://anc.bbcook.cn

[R63] 内存与进程
来源：http://vog.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://jxs.fzhhl.top

[R64] 结束进程
来源：http://eji.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://crd.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://qtf.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qlk.nwbrower.top

[R66] 定时任务
来源：http://vet.fehbvm.com

crontab -e;  crontab -l
来源：http://kzx.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://fhw.cqqwz.cn

openssl rand -hex 16
来源：http://qda.redwolf501.top

[R68] 计算文件校验值
来源：http://nnd.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://udj.zhoulong.xyz

[R69] 生成随机密码
来源：http://aqa.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://tah.tanke756.top

[R70] 时间戳与互转
来源：http://cyh.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://sij.zhengqikj.top

[R71] 日期格式化
来源：http://tjh.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hfu.guannengcc.top

[R72] 等待端口就绪
来源：http://nrh.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jel.ppjwa.cn

[R73] 分割大日志
来源：http://ifq.nwbrower.top

split -l 1000 big.log part_
来源：http://znl.jqgfzy.top

[R74] 批量重命名
来源：http://glz.fktsv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dvc.dashuyun.cn

[R75] 导出环境变量
来源：http://uyq.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://mfn.guannengcc.top

[R76] 使用临时文件
来源：http://hwr.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fdf.sufxvd.cn

[R77] 读取用户输入
来源：http://fny.jlsjyb.cn

read -rp "请输入: " ans
来源：http://sxm.ppjwa.cn

[R78] 交互式菜单
来源：http://oik.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cie.cqqwz.cn

[R79] 解析命令行选项
来源：http://ngy.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://koq.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://fyi.wangdashe.top

time ./run.sh
来源：http://ntr.zhoulong.xyz

================================================================================
来源：http://zfw.zhengqikj.top

S. C / C++ 专题
来源：http://ynq.9152youxi.cn

================================================================================
来源：http://iqj.kuanghao11.cn

[S01] C：Hello World
来源：http://ndl.yj20258888.top

#include <stdio.h>
来源：http://flr.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://gxc.daxiang520.top

[S02] C：变量与格式化输出
来源：http://zak.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://ycd.yanxiufei.cn

[S03] C：读入整数
来源：http://adm.yuanzhike.top

int x; scanf("%d", &x);
来源：http://fnf.guowangkeji.top

[S04] C：字符串复制
来源：http://xhr.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://edp.yj202588.top

[S05] C：字符串长度
来源：http://qnu.tanke756.top

strlen(s)
来源：http://vsx.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://nbl.shzxlz.cn

strcmp(a, b) == 0
来源：http://grk.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://ubs.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dop.cashguo.top

[S08] C：动态内存分配与释放
来源：http://hps.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xbz.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://yur.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eyo.smart0.xyz

[S10] C：指针与解引用
来源：http://ewt.sxryk.cn

int *p = &a;  *p = 5;
来源：http://stb.zdqjudy.top

[S11] C：逐行读文件
来源：http://fqb.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://pwm.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pnl.ybcxt.top

fclose(f);
来源：http://xkm.ivvv.top

[S12] C：写文件
来源：http://wbh.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhx.ctjpmb.com

[S13] C：宏定义
来源：http://dkp.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iac.jianghu66.top

[S14] C：枚举
来源：http://sck.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://cgq.cashguo.top

[S15] C：类型转换
来源：http://joz.yfazqb.com

(double) a / b
来源：http://qoc.tian-w.cn

[S16] C：位操作置位
来源：http://pqm.0kj1m.cn

x |= (1 << 3);
来源：http://uoh.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://afs.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mcu.xuetiantiany.cn

[S18] C：命令行参数
来源：http://zbl.hcnkem.com

int main(int argc, char **argv)
来源：http://hmg.jyoumei.cn

[S19] C：快速排序
来源：http://oip.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nlk.bjfxy.top

[S20] C：二分查找
来源：http://fxy.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://puu.ivvv.top

[S21] C：字符类别判断
来源：http://dop.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vdw.yvedp.cn

[S22] C：字符串转数字
来源：http://jos.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://odq.feifeiyinyue.top

[S23] C：随机数
来源：http://qyu.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://vts.epnwcf.com

[S24] C：获取本地时间
来源：http://rxa.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mrr.316326.xyz

[S25] C：内存拷贝
来源：http://qgd.yvedp.cn

memcpy(dst, src, n);
来源：http://hpx.ydjk.org.cn

[S26] C：内存清零
来源：http://zpw.smart0.xyz

memset(a, 0, sizeof a);
来源：http://xam.pycfn.com

[S27] C：定义常量
来源：http://dlj.dianchejie.cn

const double PI = 3.14159;
来源：http://ktd.havefunace.top

[S28] C：静态变量
来源：http://mmx.yj202588.top

static int counter = 0;
来源：http://ghf.jlsjyb.cn

[S29] C：变参函数
来源：http://sii.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gsu.zhijiandao.cn

[S30] C：头文件保护
来源：http://jin.pengpengdd.cyou

#ifndef X_H
来源：http://yln.ivvv.top

#define X_H
来源：http://btc.zhaomingkeji.xyz

#endif
来源：http://bag.ivvv.top

[S31] C++：Hello World
来源：http://kzg.0kj1m.cn

#include <iostream>
来源：http://kah.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://ice.sjlbkw.cn

[S32] C++：字符串
来源：http://zqp.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://soa.nanxuanxn.top

[S33] C++：vector 增删
来源：http://trc.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://plx.hcnkem.com

[S34] C++：遍历 vector
来源：http://aml.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://nah.fktsv.cn

[S35] C++：map
来源：http://hac.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://slp.yongpay.top

[S36] C++：unordered_map
来源：http://iuw.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lka.redwolf501.top

[S37] C++：set
来源：http://ijr.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ygl.hfpthk.cn

[S38] C++：排序
来源：http://dzj.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://xvx.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://ehk.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://myj.gogol.net.cn

[S40] C++：查找元素
来源：http://rpd.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://phv.birdmap.top

[S41] C++：类与构造函数
来源：http://adl.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pnb.xinyue.icu

[S42] C++：继承与虚函数
来源：http://ncy.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://jgy.52xcode.cn


<!-- 参考信息 -->