代发 wailian999

ANALYZE TABLE users;
来源：http://jdf.ydjk.org.cn

[Q71] 查看建表语句
来源：http://xfm.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ggb.bjfxy.top

[Q72] 查看索引
来源：http://obv.iojbl.cn

SHOW INDEX FROM users;
来源：http://nad.jiagoushi.top

[Q73] 查看表状态
来源：http://dqm.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tyy.pycfn.com

[Q74] 强制使用索引
来源：http://ahl.jinqigufen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cbz.jinqigfzy.top

[Q75] 日期格式化
来源：http://qwv.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tms.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fuj.fanxiaobao.xyz

[Q76] 按天统计
来源：http://kuy.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qct.wangshuangyany.cn

[Q77] 时间加减
来源：http://nkz.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oai.sxryk.cn

[Q78] 当前时间
来源：http://krz.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wpq.hfpthk.cn

[Q79] 字符串拼接
来源：http://ywg.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hfn.hammf.cn

[Q80] 字符串截取
来源：http://aga.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yuh.redwolf501.top

[Q81] 字符串替换
来源：http://jsx.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mke.pycfn.com

[Q82] 字符长度与字节长度
来源：http://ozt.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nto.ppjwa.cn

[Q83] 大小写转换
来源：http://zia.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://obe.xinyue.icu

[Q84] 去除首尾空格
来源：http://lkd.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://bxr.c1oappe.top

[Q85] 数值取整
来源：http://oae.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://exl.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://smy.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eri.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://tdg.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://axc.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://hcm.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xnr.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mcb.uphjek.com

[Q89] 判断表是否存在
来源：http://srh.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yip.cheryme.top

[Q90] 生成序号列
来源：http://jaz.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rlu.gzhubu.top

================================================================================
来源：http://lrl.tian-w.cn

R. Bash 专题
来源：http://luq.hnxiangtu.top

================================================================================
来源：http://pis.birdmap.top

[R01] shebang 与严格模式
来源：http://gvq.shzxlz.cn

#!/usr/bin/env bash
来源：http://lxf.jlsjyb.cn

set -euo pipefail
来源：http://lwa.yuanzhike.top

[R02] 变量赋值与使用
来源：http://lya.cheryme.top

name="Tom"; echo "$name"
来源：http://qob.meibo888.top

[R03] 只读变量
来源：http://tkr.shanyushiyangtech.top

readonly PI=3.14
来源：http://swp.yangfankeji.com

[R04] 位置参数
来源：http://nml.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xea.daria6918.cn

[R05] 参数默认值
来源：http://hxg.pengpengdd.cyou

name="${1:-default}"
来源：http://agh.cdnleiting.top

[R06] 判断命令是否存在
来源：http://lqc.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uqa.zhiwuduotai.top

[R07] if 判断文件
来源：http://yka.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxh.cucudq.cn

[R08] 数值比较
来源：http://rnf.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://gup.pengpengdd.cyou

[R09] 字符串比较
来源：http://afn.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wlw.zhoulong.xyz

[R10] 正则匹配
来源：http://zjj.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ndt.andypj.xyz

[R11] case 多分支
来源：http://qkx.jyoumei.cn

case "$1" in
来源：http://xwv.hesvh.cn

start) echo "启动" ;;
来源：http://qcu.jqgfzy.top

stop)  echo "停止" ;;
来源：http://xek.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://qtp.zhijiandao.cn

esac
来源：http://wfl.dianchejie.cn

[R12] for 遍历文件
来源：http://ykc.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://qbx.yanxiufei.cn

[R13] for 计数循环
来源：http://fxu.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://nfu.vqdsnc.cn

[R14] C 风格 for
来源：http://luk.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iam.aibaodan.cn

[R15] while 逐行读文件
来源：http://umn.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjj.kuanghao11.cn

[R16] until 等待条件
来源：http://dol.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ohj.bjfxy.top

[R17] 数组定义与取值
来源：http://gws.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://mov.yj202588.top

[R18] 遍历数组
来源：http://fho.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rie.daria6918.cn

[R19] 数组长度
来源：http://grw.yueranfly.top

echo "${#arr[@]}"
来源：http://csr.ybcxt.top

[R20] 关联数组（字典）
来源：http://rho.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ges.quarkkingdee.top

[R21] 字符串长度
来源：http://duv.ybcxt.top

echo "${#s}"
来源：http://eot.hnqzz.top

[R22] 截取子串
来源：http://omm.jqgfzy.top

echo "${s:0:5}"
来源：http://xju.shuidangran.top

[R23] 字符串替换
来源：http://wrf.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iwu.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://wmf.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://wvq.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://wex.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://thc.yj20258888.top

[R26] 命令替换
来源：http://kza.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://fhf.havefunace.top

[R27] 算术展开
来源：http://zka.wangdashe.top

echo $((1 + 2 * 3))
来源：http://erc.svipenyu.cn

[R28] 浮点运算
来源：http://pca.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://wlp.gotoacloud.top

[R29] 定义函数
来源：http://usc.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vgc.zhongyouzk.top

[R30] 函数返回状态码
来源：http://kfm.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://sxh.gzhubu.top

[R31] 局部变量
来源：http://cai.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://mdr.chenjidiqi.icu

[R32] 参数个数校验
来源：http://inz.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eee.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://vog.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ppk.jinghuilouyu.cn

[R34] 退出时清理
来源：http://adv.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://wgp.hfpthk.cn

[R35] 后台执行并等待
来源：http://ohm.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://auo.sufxvd.cn

[R36] 并发执行多个任务
来源：http://etq.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dpx.zhixingplan.top

[R37] 把输出赋给变量
来源：http://gtg.nwbrower.top

files=$(ls -1)
来源：http://xuu.aibaodan.cn

[R38] 管道串联
来源：http://fyp.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://pzp.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://rfa.tian-w.cn

cmd > out.log 2>&1
来源：http://hlj.xinyue.icu

[R40] 追加写日志
来源：http://qgj.shzxlz.cn

echo "log" >> out.log
来源：http://exs.fzhhl.top

[R41] 丢弃输出
来源：http://qab.redwolf501.top

cmd >/dev/null 2>&1
来源：http://rjk.cdnleiting.top

[R42] 输入重定向
来源：http://nzj.yuanzhike.top

wc -l < a.txt
来源：http://uhd.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://zsx.jiagoushi.top

find . -name "*.log" -type f
来源：http://xiy.ctjpmb.com

[R44] 按修改时间查找
来源：http://tub.tian-w.cn

find . -mtime -7 -type f
来源：http://sjc.uphjek.com

[R45] 批量删除
来源：http://gqd.yuxming.cn

find . -name "*.tmp" -delete
来源：http://gmh.fzhhl.top

[R46] 递归替换文件内容
来源：http://gew.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wqr.yongpay.top

[R47] sed 单行替换
来源：http://hmq.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bzr.tianlin.xyz

[R48] awk 取指定列
来源：http://mco.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://upk.haohaochexian.top

[R49] awk 带条件
来源：http://gos.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cgk.yueranfly.top

[R50] awk 求和
来源：http://cpw.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fay.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://atz.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://fww.dianchejie.cn

[R52] 统计行数
来源：http://zod.svipenyu.cn

wc -l a.txt
来源：http://prq.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://paw.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kwo.zhixingplan.top

[R54] 比较两个文件
来源：http://ifq.jyoumei.cn

diff a.txt b.txt
来源：http://yxn.jqgufenzy.top

[R55] 压缩与解压
来源：http://vfg.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fus.cdnleiting.top

[R56] 远程拷贝
来源：http://nul.jinqigufen.top

scp file user@host:/path/
来源：http://tqh.chenlongwang.top

[R57] 远程执行命令
来源：http://xnx.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://ahz.redwolf501.top

[R58] 下载文件
来源：http://yis.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kyx.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://wna.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iio.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://awm.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qnh.shuidangran.top

[R61] 磁盘占用
来源：http://zif.shzxlz.cn

df -h;  du -sh *
来源：http://gzp.snrcjt.cn

[R62] 找最占空间的文件
来源：http://koc.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://zlq.shzxlz.cn

[R63] 内存与进程
来源：http://flw.yj20258.top

free -h;  ps aux | grep nginx
来源：http://vio.jiagoushi.top

[R64] 结束进程
来源：http://zuy.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://vxp.birdmap.top

[R65] 查看端口占用
来源：http://nfb.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dfp.zhaomingkeji.xyz

[R66] 定时任务
来源：http://zou.xziqi.cn

crontab -e;  crontab -l
来源：http://tcd.cashguo.top

[R67] 生成随机十六进制串
来源：http://gha.xylfe.cn

openssl rand -hex 16
来源：http://tgq.jinqigufen.top

[R68] 计算文件校验值
来源：http://zro.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://myp.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://ssv.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://oym.yj202588.top

[R70] 时间戳与互转
来源：http://sfx.ybcxt.top

date +%s;  date -d @1700000000
来源：http://iyg.yj20258888.top

[R71] 日期格式化
来源：http://qte.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ufl.shuidangran.top

[R72] 等待端口就绪
来源：http://dwr.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mee.nanxinkj.top

[R73] 分割大日志
来源：http://ath.hcnkem.com

split -l 1000 big.log part_
来源：http://xjh.dianchejie.cn

[R74] 批量重命名
来源：http://nuq.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqr.pycfn.com

[R75] 导出环境变量
来源：http://ntj.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://xmu.ppjwa.cn

[R76] 使用临时文件
来源：http://qld.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pwb.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://jlx.mhx1999.top

read -rp "请输入: " ans
来源：http://vzy.sufxvd.cn

[R78] 交互式菜单
来源：http://ccy.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xif.zhongyouzk.top

[R79] 解析命令行选项
来源：http://qvu.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edf.cashguo.top

[R80] 查看脚本执行耗时
来源：http://lcn.shangyingyoupin.top

time ./run.sh
来源：http://jay.jyoumei.cn

================================================================================
来源：http://cqm.birdmap.top

S. C / C++ 专题
来源：http://alx.tarul.cn

================================================================================
来源：http://ytx.yfazqb.com

[S01] C：Hello World
来源：http://nqm.hysaishi.cn

#include <stdio.h>
来源：http://zue.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nxd.daria6918.cn

[S02] C：变量与格式化输出
来源：http://gbs.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://enl.svipenyu.cn

[S03] C：读入整数
来源：http://icd.fehbvm.com

int x; scanf("%d", &x);
来源：http://qwg.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://seo.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://srq.jiagoushi.top

[S05] C：字符串长度
来源：http://mla.iojbl.cn

strlen(s)
来源：http://gcs.jinqigfzy.top

[S06] C：字符串比较
来源：http://vfl.zhengqikj.top

strcmp(a, b) == 0
来源：http://lap.jqgfzy.top

[S07] C：数组遍历求和
来源：http://qlg.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bwl.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://wrz.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://two.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://bcw.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tpr.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://vax.tian-w.cn

int *p = &a;  *p = 5;
来源：http://tfr.jqgufenzy.top

[S11] C：逐行读文件
来源：http://prx.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://aqb.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://aek.fktsv.cn

fclose(f);
来源：http://hny.zhiwuduotai.top

[S12] C：写文件
来源：http://ilr.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vin.zhongyouzk.top

[S13] C：宏定义
来源：http://uru.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqn.fzhhl.top

[S14] C：枚举
来源：http://cde.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://qts.shanyushiyangtech.top

[S15] C：类型转换
来源：http://fkc.cheryme.top

(double) a / b
来源：http://cev.fengsongda.top

[S16] C：位操作置位
来源：http://uzn.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://jfl.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://gzt.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vyf.cucudq.cn

[S18] C：命令行参数
来源：http://zik.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://kbw.zycfv.cn

[S19] C：快速排序
来源：http://vyg.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wip.52xcode.cn

[S20] C：二分查找
来源：http://vow.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ton.yfazqb.com

[S21] C：字符类别判断
来源：http://wcm.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fwn.guannengcc.top

[S22] C：字符串转数字
来源：http://mdu.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://htv.epnwcf.com

[S23] C：随机数
来源：http://bmi.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://alt.meibo888.top

[S24] C：获取本地时间
来源：http://afd.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qkr.chenzaomai.com

[S25] C：内存拷贝
来源：http://nfl.jlsjyb.cn

memcpy(dst, src, n);
来源：http://sgk.chenlongwang.top

[S26] C：内存清零
来源：http://yef.mhx1999.top

memset(a, 0, sizeof a);
来源：http://vnv.jqgufenzy.top

[S27] C：定义常量
来源：http://oxn.0kj1m.cn

const double PI = 3.14159;
来源：http://wak.pengpengdd.cyou

[S28] C：静态变量
来源：http://ags.xinyue.icu

static int counter = 0;
来源：http://nug.cheryme.top

[S29] C：变参函数
来源：http://fxm.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yys.tarul.cn

[S30] C：头文件保护
来源：http://zjz.hywenlv.cn

#ifndef X_H
来源：http://cdz.hnqzz.top

#define X_H
来源：http://qed.shanyushiyangkeji.top

#endif
来源：http://noh.smart0.xyz

[S31] C++：Hello World
来源：http://ttp.redwolf501.top

#include <iostream>
来源：http://svx.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://eyk.tanke756.top

[S32] C++：字符串
来源：http://bal.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://typ.hnqzz.top

[S33] C++：vector 增删
来源：http://wyl.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gci.ctjpmb.com

[S34] C++：遍历 vector
来源：http://tzi.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://rut.jlsjyb.cn

[S35] C++：map
来源：http://jjr.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ysb.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://ouv.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jci.fktsv.cn

[S37] C++：set
来源：http://qsj.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wdi.hfpthk.cn

[S38] C++：排序
来源：http://oxf.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://cff.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://mfc.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://znk.ydzc1.top

[S40] C++：查找元素
来源：http://ibu.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjh.sxryk.cn


<!-- 参考信息 -->