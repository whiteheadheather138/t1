代发 wailian999

SHOW INDEX FROM users;
来源：http://ctd.ivvv.top

[Q73] 查看表状态
来源：http://mcy.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ekl.hesvh.cn

[Q74] 强制使用索引
来源：http://iqm.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qxl.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://mjz.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eap.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hed.cdnleiting.top

[Q76] 按天统计
来源：http://aaq.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://euy.uphjek.com

[Q77] 时间加减
来源：http://sia.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mnz.kuanghao11.cn

[Q78] 当前时间
来源：http://udi.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ojh.jianghu66.top

[Q79] 字符串拼接
来源：http://ejt.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ooq.xuetiantiany.cn

[Q80] 字符串截取
来源：http://lab.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wrm.hysaishi.cn

[Q81] 字符串替换
来源：http://fjz.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xyy.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://phd.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ygs.gotoacloud.top

[Q83] 大小写转换
来源：http://bgw.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://krx.zhengqikj.top

[Q84] 去除首尾空格
来源：http://rps.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://aed.fengsongda.top

[Q85] 数值取整
来源：http://hlz.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lhj.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://rnq.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iki.yvedp.cn

[Q87] JSON 字段做条件
来源：http://eng.fzhhl.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nyn.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://aft.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ejd.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://syr.cashguo.top

[Q89] 判断表是否存在
来源：http://mvh.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xmy.yangfankeji.com

[Q90] 生成序号列
来源：http://mnj.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vxy.uphjek.com

================================================================================
来源：http://qgw.c1oappe.top

R. Bash 专题
来源：http://aes.chenzaomai.com

================================================================================
来源：http://sey.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://hgp.jlsjyb.cn

#!/usr/bin/env bash
来源：http://ugv.zdqjudy.top

set -euo pipefail
来源：http://lqe.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://kre.jiagoushi.top

name="Tom"; echo "$name"
来源：http://bxh.redwolf501.top

[R03] 只读变量
来源：http://kpa.gaohongyu789.top

readonly PI=3.14
来源：http://rrb.quarkkingdee.top

[R04] 位置参数
来源：http://uuo.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nok.iojbl.cn

[R05] 参数默认值
来源：http://zuo.epnwcf.com

name="${1:-default}"
来源：http://jas.tanke756.top

[R06] 判断命令是否存在
来源：http://alj.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bge.dashuyun.cn

[R07] if 判断文件
来源：http://ugw.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eed.pycfn.com

[R08] 数值比较
来源：http://tmr.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zps.xuetiantiany.cn

[R09] 字符串比较
来源：http://klz.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nwt.zhixingplan.top

[R10] 正则匹配
来源：http://faf.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dcw.gzhubu.top

[R11] case 多分支
来源：http://efj.hywenlv.cn

case "$1" in
来源：http://jfr.jqgufenzy.top

start) echo "启动" ;;
来源：http://zux.cqqwz.cn

stop)  echo "停止" ;;
来源：http://jlc.ivvv.top

*)     echo "未知命令" ;;
来源：http://bdv.cdnleiting.top

esac
来源：http://zte.yj202588.top

[R12] for 遍历文件
来源：http://kug.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://hlc.0kj1m.cn

[R13] for 计数循环
来源：http://lgf.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://irj.yj20258888.top

[R14] C 风格 for
来源：http://wqr.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nug.aizwys.cn

[R15] while 逐行读文件
来源：http://kvn.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tox.shzxlz.cn

[R16] until 等待条件
来源：http://fou.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ckl.yj20258888.top

[R17] 数组定义与取值
来源：http://ddj.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://spl.yanxiufei.cn

[R18] 遍历数组
来源：http://jgr.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tkt.shzxlz.cn

[R19] 数组长度
来源：http://vxr.ppjwa.cn

echo "${#arr[@]}"
来源：http://drm.ybcxt.top

[R20] 关联数组（字典）
来源：http://jzv.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iqn.fengsongda.top

[R21] 字符串长度
来源：http://yxh.dashuyun.cn

echo "${#s}"
来源：http://rvu.yfazqb.com

[R22] 截取子串
来源：http://xei.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://pnh.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://drg.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mua.0kj1m.cn

[R24] 大小写转换
来源：http://jzr.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://hal.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://pxp.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ftu.pycfn.com

[R26] 命令替换
来源：http://fev.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://twi.hysaishi.cn

[R27] 算术展开
来源：http://tvy.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://ypu.jianghu66.top

[R28] 浮点运算
来源：http://oxd.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://trg.ydzc1.top

[R29] 定义函数
来源：http://nbs.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zok.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://pcj.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://pjm.0kj1m.cn

[R31] 局部变量
来源：http://lam.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://ahe.zdqjudy.top

[R32] 参数个数校验
来源：http://cmg.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ooh.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://fxq.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cvj.vqdsnc.cn

[R34] 退出时清理
来源：http://jab.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://cvs.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://ojd.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qtv.cdnleiting.top

[R36] 并发执行多个任务
来源：http://cly.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tfh.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://bxj.jinqigufen.top

files=$(ls -1)
来源：http://prm.hfpthk.cn

[R38] 管道串联
来源：http://lsx.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://yst.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://icq.zycfv.cn

cmd > out.log 2>&1
来源：http://anp.zhongyouzk.top

[R40] 追加写日志
来源：http://bhg.svipenyu.cn

echo "log" >> out.log
来源：http://sbu.wangshuangyany.cn

[R41] 丢弃输出
来源：http://sky.nwbrower.top

cmd >/dev/null 2>&1
来源：http://vmx.gotoacloud.top

[R42] 输入重定向
来源：http://lqp.yj20258888.top

wc -l < a.txt
来源：http://sgr.hnxiangtu.top

[R43] 按名字查找文件
来源：http://une.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://nri.nanxuanxn.top

[R44] 按修改时间查找
来源：http://pyt.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://blm.chenlongwang.top

[R45] 批量删除
来源：http://fzm.52xcode.cn

find . -name "*.tmp" -delete
来源：http://cci.cucudq.cn

[R46] 递归替换文件内容
来源：http://rnc.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kqf.pengpengdd.cyou

[R47] sed 单行替换
来源：http://huy.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://cdy.sysykeji.top

[R48] awk 取指定列
来源：http://bjz.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://yom.jyoumei.cn

[R49] awk 带条件
来源：http://fip.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rto.fanxiaobao.xyz

[R50] awk 求和
来源：http://bug.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://fnr.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://hof.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ydb.gogol.net.cn

[R52] 统计行数
来源：http://cpl.gzhubu.top

wc -l a.txt
来源：http://yed.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://jmy.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iax.pengpengdd.cyou

[R54] 比较两个文件
来源：http://pld.kuanghao11.cn

diff a.txt b.txt
来源：http://ijd.hysaishi.cn

[R55] 压缩与解压
来源：http://sgs.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ygh.cashguo.top

[R56] 远程拷贝
来源：http://ghx.epnwcf.com

scp file user@host:/path/
来源：http://hrv.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://ecf.iojbl.cn

ssh user@host 'uptime'
来源：http://eqb.gzhubu.top

[R58] 下载文件
来源：http://qee.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggq.quarkkingdee.top

[R59] 发 POST JSON
来源：http://gnh.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zyj.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://enc.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://obb.gzhubu.top

[R61] 磁盘占用
来源：http://isz.smart0.xyz

df -h;  du -sh *
来源：http://wow.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://zlj.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://odp.daria6918.cn

[R63] 内存与进程
来源：http://lli.ivvv.top

free -h;  ps aux | grep nginx
来源：http://zwy.dianchejie.cn

[R64] 结束进程
来源：http://ije.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://gkh.yj20258888.top

[R65] 查看端口占用
来源：http://frh.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ypq.ctjpmb.com

[R66] 定时任务
来源：http://fyn.hammf.cn

crontab -e;  crontab -l
来源：http://nel.tian-w.cn

[R67] 生成随机十六进制串
来源：http://qun.cucudq.cn

openssl rand -hex 16
来源：http://auz.xuanzx.com

[R68] 计算文件校验值
来源：http://wtj.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fnm.vqdsnc.cn

[R69] 生成随机密码
来源：http://vdf.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://qvu.9152youxi.cn

[R70] 时间戳与互转
来源：http://gha.bjfxy.top

date +%s;  date -d @1700000000
来源：http://qja.yfazqb.com

[R71] 日期格式化
来源：http://nrf.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tsg.tian-w.cn

[R72] 等待端口就绪
来源：http://qtf.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vnq.aibaodan.cn

[R73] 分割大日志
来源：http://kfz.shzxlz.cn

split -l 1000 big.log part_
来源：http://nzd.tanke756.top

[R74] 批量重命名
来源：http://xqx.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://evo.9152youxi.cn

[R75] 导出环境变量
来源：http://kmv.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://fac.ctjpmb.com

[R76] 使用临时文件
来源：http://xez.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utp.jqgufenzy.top

[R77] 读取用户输入
来源：http://rpi.fktsv.cn

read -rp "请输入: " ans
来源：http://nmf.hnqzz.top

[R78] 交互式菜单
来源：http://jsp.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ymk.nwbrower.top

[R79] 解析命令行选项
来源：http://mcp.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://adb.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wem.ydzc1.top

time ./run.sh
来源：http://kdb.zhixingplan.top

================================================================================
来源：http://wyo.chenzaomai.com

S. C / C++ 专题
来源：http://nab.cucudq.cn

================================================================================
来源：http://yus.tanke756.top

[S01] C：Hello World
来源：http://oic.vehdjk.com

#include <stdio.h>
来源：http://nsp.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uay.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://ahw.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://rdo.hysaishi.cn

[S03] C：读入整数
来源：http://brc.dianchejie.cn

int x; scanf("%d", &x);
来源：http://agb.haohaochexian.top

[S04] C：字符串复制
来源：http://tca.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vsh.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://gfj.birdmap.top

strlen(s)
来源：http://nbp.vehdjk.com

[S06] C：字符串比较
来源：http://ekz.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://qds.yongpay.top

[S07] C：数组遍历求和
来源：http://mrj.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://whn.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://epj.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://csb.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://uul.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rgp.yuxming.cn

[S10] C：指针与解引用
来源：http://ppg.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://nkf.hywenlv.cn

[S11] C：逐行读文件
来源：http://tzf.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvz.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kuy.sweek.top

fclose(f);
来源：http://jds.kuanghao11.cn

[S12] C：写文件
来源：http://eex.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hgv.daria6918.cn

[S13] C：宏定义
来源：http://xav.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqd.316326.xyz

[S14] C：枚举
来源：http://tmr.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://quq.jyoumei.cn

[S15] C：类型转换
来源：http://mhv.jinqigfzy.top

(double) a / b
来源：http://kia.sysykeji.top

[S16] C：位操作置位
来源：http://zpa.yj20258.top

x |= (1 << 3);
来源：http://yxv.yj202588.top

[S17] C：安全拼接字符串
来源：http://mug.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gmm.tianlin.xyz

[S18] C：命令行参数
来源：http://foh.daria6918.cn

int main(int argc, char **argv)
来源：http://olv.ivvv.top

[S19] C：快速排序
来源：http://wie.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://wkf.ehwqpu.com

[S20] C：二分查找
来源：http://xck.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rqn.vqdsnc.cn

[S21] C：字符类别判断
来源：http://ice.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mxr.sweek.top

[S22] C：字符串转数字
来源：http://rpd.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://xtd.ctjpmb.com

[S23] C：随机数
来源：http://mcz.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tji.sxryk.cn

[S24] C：获取本地时间
来源：http://hgm.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yax.bbcook.cn

[S25] C：内存拷贝
来源：http://cij.uphjek.com

memcpy(dst, src, n);
来源：http://cpg.ybcxt.top

[S26] C：内存清零
来源：http://gme.pycfn.com

memset(a, 0, sizeof a);
来源：http://jcw.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://lqm.daria6918.cn

const double PI = 3.14159;
来源：http://hbz.tanke756.top

[S28] C：静态变量
来源：http://niu.sufxvd.cn

static int counter = 0;
来源：http://pdj.jiagoushi.top

[S29] C：变参函数
来源：http://ldy.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jab.bjfxy.top

[S30] C：头文件保护
来源：http://ziz.yonumen.top

#ifndef X_H
来源：http://chn.fzhhl.top

#define X_H
来源：http://ljp.quarkkingdee.top

#endif
来源：http://sqf.zhoulong.xyz

[S31] C++：Hello World
来源：http://hcw.snrcjt.cn

#include <iostream>
来源：http://ezg.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://lbv.gzhubu.top

[S32] C++：字符串
来源：http://vqk.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://lbg.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://bzj.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ijk.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://bhl.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://ysk.yfazqb.com

[S35] C++：map
来源：http://ysz.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cas.yonumen.top

[S36] C++：unordered_map
来源：http://fpp.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://omt.xuanzx.com

[S37] C++：set
来源：http://wuf.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxs.guowangkeji.top

[S38] C++：排序
来源：http://jjb.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://tbn.yonumen.top

[S39] C++：自定义比较器排序
来源：http://xnv.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yav.hongshengwenyu.top

[S40] C++：查找元素
来源：http://itb.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oze.sxryk.cn

[S41] C++：类与构造函数
来源：http://gkc.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mzt.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://rmi.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://fuw.aibaodan.cn


<!-- 参考信息 -->