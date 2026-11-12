代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tye.zdqjudy.top

[Q58] 累计求和
来源：http://tsk.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://owl.yongpay.top

[Q59] 分组内累计
来源：http://kpq.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://phl.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://jhj.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eak.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hsq.zhongyouzk.top

[Q61] 移动平均
来源：http://wsl.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eyq.birdmap.top

[Q62] 分组占比
来源：http://huo.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwn.iojbl.cn

[Q63] 开启事务
来源：http://cor.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zlf.guannengcc.top

[Q64] 提交事务
来源：http://fql.ppjwa.cn

COMMIT;
来源：http://ktp.hfpthk.cn

[Q65] 回滚事务
来源：http://nxb.andypj.xyz

ROLLBACK;
来源：http://hdn.pycfn.com

[Q66] 行锁查询
来源：http://sgn.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kjk.wangshuangyany.cn

[Q67] 设置隔离级别
来源：http://tnr.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ufr.52xcode.cn

[Q68] 保存点
来源：http://uaq.bjfxy.top

SAVEPOINT sp1;
来源：http://zsd.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://olo.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://ohg.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://njn.jlsjyb.cn

[Q70] 更新统计信息
来源：http://vgb.yongpay.top

ANALYZE TABLE users;
来源：http://fkw.hfpthk.cn

[Q71] 查看建表语句
来源：http://vnt.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qzw.wangshuangyany.cn

[Q72] 查看索引
来源：http://rin.bjfxy.top

SHOW INDEX FROM users;
来源：http://rin.gotoacloud.top

[Q73] 查看表状态
来源：http://zph.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vjg.hesvh.cn

[Q74] 强制使用索引
来源：http://ema.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikv.jqgufenzy.top

[Q75] 日期格式化
来源：http://nwf.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aps.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lrx.tianlin.xyz

[Q76] 按天统计
来源：http://ajj.ydzc1.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ege.pengpengdd.cyou

[Q77] 时间加减
来源：http://jbc.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://loy.yueranfly.top

[Q78] 当前时间
来源：http://stw.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tvk.fengsongda.top

[Q79] 字符串拼接
来源：http://hvl.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bmn.316326.xyz

[Q80] 字符串截取
来源：http://cqn.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://amg.xinyue.icu

[Q81] 字符串替换
来源：http://wko.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kok.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://qko.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rnq.hnqzz.top

[Q83] 大小写转换
来源：http://kon.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://olr.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://jft.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://gyl.cheryme.top

[Q85] 数值取整
来源：http://jqh.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ncc.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://bjk.birdmap.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gtp.52xcode.cn

[Q87] JSON 字段做条件
来源：http://vvr.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zcd.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://gdd.xylfe.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fky.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nnn.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://fye.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nwt.epnwcf.com

[Q90] 生成序号列
来源：http://yja.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://egl.cqqwz.cn

================================================================================
来源：http://quq.hywenlv.cn

R. Bash 专题
来源：http://gkh.yj20258.top

================================================================================
来源：http://eth.chenzaomai.com

[R01] shebang 与严格模式
来源：http://sue.zdbjq.cn

#!/usr/bin/env bash
来源：http://mpp.cucudq.cn

set -euo pipefail
来源：http://luj.fehbvm.com

[R02] 变量赋值与使用
来源：http://mar.zhixingplan.top

name="Tom"; echo "$name"
来源：http://mxf.sysykeji.top

[R03] 只读变量
来源：http://inz.daria6918.cn

readonly PI=3.14
来源：http://pgy.ppjwa.cn

[R04] 位置参数
来源：http://uyk.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vtk.shangyingyoupin.top

[R05] 参数默认值
来源：http://wse.316326.xyz

name="${1:-default}"
来源：http://fti.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://uke.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zhe.ybcxt.top

[R07] if 判断文件
来源：http://ruy.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://moh.quarkkingdee.top

[R08] 数值比较
来源：http://cyj.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hes.zhengqikj.top

[R09] 字符串比较
来源：http://jru.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jjw.meibo888.top

[R10] 正则匹配
来源：http://nld.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ztu.gotoacloud.top

[R11] case 多分支
来源：http://hyu.uphjek.com

case "$1" in
来源：http://kij.dianchejie.cn

start) echo "启动" ;;
来源：http://bch.yongpay.top

stop)  echo "停止" ;;
来源：http://ozq.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://erf.cucudq.cn

esac
来源：http://geq.316326.xyz

[R12] for 遍历文件
来源：http://yah.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://tdm.ydjk.org.cn

[R13] for 计数循环
来源：http://bzz.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://dkk.tanke756.top

[R14] C 风格 for
来源：http://jcj.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fno.yuxming.cn

[R15] while 逐行读文件
来源：http://rbb.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nff.snrcjt.cn

[R16] until 等待条件
来源：http://nzx.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ljz.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://hwx.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://tqf.andypj.xyz

[R18] 遍历数组
来源：http://pum.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vgr.tanke756.top

[R19] 数组长度
来源：http://qzv.zhixingplan.top

echo "${#arr[@]}"
来源：http://kzy.pycfn.com

[R20] 关联数组（字典）
来源：http://hhp.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://slh.dianchejie.cn

[R21] 字符串长度
来源：http://qmu.gotoacloud.top

echo "${#s}"
来源：http://cnp.daria6918.cn

[R22] 截取子串
来源：http://ttw.yj20258.top

echo "${s:0:5}"
来源：http://oqe.meibo888.top

[R23] 字符串替换
来源：http://fsn.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cnl.svipenyu.cn

[R24] 大小写转换
来源：http://izl.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://trm.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://rqd.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehe.shangyingyoupin.top

[R26] 命令替换
来源：http://jei.yonumen.top

now=$(date +%F); echo "$now"
来源：http://isv.redwolf501.top

[R27] 算术展开
来源：http://xnt.redwolf501.top

echo $((1 + 2 * 3))
来源：http://vtg.cashguo.top

[R28] 浮点运算
来源：http://mde.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://ezz.yvedp.cn

[R29] 定义函数
来源：http://oma.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xen.bbcook.cn

[R30] 函数返回状态码
来源：http://nns.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://mht.yj20258888.top

[R31] 局部变量
来源：http://ohx.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://tha.yonumen.top

[R32] 参数个数校验
来源：http://qsq.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sbb.tarul.cn

[R33] 捕获错误并提示行号
来源：http://crd.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tce.yanxiufei.cn

[R34] 退出时清理
来源：http://pqu.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mdm.havefunace.top

[R35] 后台执行并等待
来源：http://iqo.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rxw.yuanzhike.top

[R36] 并发执行多个任务
来源：http://hdw.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sdr.zdqjudy.top

[R37] 把输出赋给变量
来源：http://nbm.smart0.xyz

files=$(ls -1)
来源：http://xor.fengsongda.top

[R38] 管道串联
来源：http://zad.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://wcp.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://dit.fktsv.cn

cmd > out.log 2>&1
来源：http://grt.feifeiyinyue.top

[R40] 追加写日志
来源：http://ckl.vqdsnc.cn

echo "log" >> out.log
来源：http://vch.snrcjt.cn

[R41] 丢弃输出
来源：http://vcr.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://lgk.c1oappe.top

[R42] 输入重定向
来源：http://qae.cucudq.cn

wc -l < a.txt
来源：http://twg.yj202588.top

[R43] 按名字查找文件
来源：http://njm.fehbvm.com

find . -name "*.log" -type f
来源：http://uuv.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://ooq.cheryme.top

find . -mtime -7 -type f
来源：http://oqv.hnxiangtu.top

[R45] 批量删除
来源：http://kgh.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://xyz.9152youxi.cn

[R46] 递归替换文件内容
来源：http://fwv.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://idd.nanxinkj.top

[R47] sed 单行替换
来源：http://ltr.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://ebx.jinqigufen.top

[R48] awk 取指定列
来源：http://rnd.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://zmc.birdmap.top

[R49] awk 带条件
来源：http://ddz.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sxw.fehbvm.com

[R50] awk 求和
来源：http://qri.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qlx.havefunace.top

[R51] 排序去重取前几
来源：http://bjw.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://mir.jqgfzy.top

[R52] 统计行数
来源：http://pci.zhongyouzk.top

wc -l a.txt
来源：http://qwf.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://fcc.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fbz.hammf.cn

[R54] 比较两个文件
来源：http://yau.aibaodan.cn

diff a.txt b.txt
来源：http://yhq.guowangkeji.top

[R55] 压缩与解压
来源：http://aja.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zaa.hnxiangtu.top

[R56] 远程拷贝
来源：http://tjn.jiagoushi.top

scp file user@host:/path/
来源：http://iht.hysaishi.cn

[R57] 远程执行命令
来源：http://gaq.zhoulong.xyz

ssh user@host 'uptime'
来源：http://ysd.zycfv.cn

[R58] 下载文件
来源：http://kab.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yyb.wangdashe.top

[R59] 发 POST JSON
来源：http://fkg.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jac.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://efy.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nbh.birdmap.top

[R61] 磁盘占用
来源：http://apf.chenlongwang.top

df -h;  du -sh *
来源：http://lfd.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://dfs.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://qtv.zhiwuduotai.top

[R63] 内存与进程
来源：http://arj.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://uon.bbcook.cn

[R64] 结束进程
来源：http://nkm.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://fhw.52xcode.cn

[R65] 查看端口占用
来源：http://faw.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tuk.gzhubu.top

[R66] 定时任务
来源：http://cyd.vehdjk.com

crontab -e;  crontab -l
来源：http://cex.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://pig.9152youxi.cn

openssl rand -hex 16
来源：http://wkh.hfpthk.cn

[R68] 计算文件校验值
来源：http://sms.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iet.sjlbkw.cn

[R69] 生成随机密码
来源：http://vpx.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://wur.zhongyouzk.top

[R70] 时间戳与互转
来源：http://xsy.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://cwj.pycfn.com

[R71] 日期格式化
来源：http://ztf.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tkd.yj20258.top

[R72] 等待端口就绪
来源：http://hyg.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jhb.fanxiaobao.xyz

[R73] 分割大日志
来源：http://cxm.dashuyun.cn

split -l 1000 big.log part_
来源：http://vov.chenlongwang.top

[R74] 批量重命名
来源：http://lac.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cgr.chenjidiqi.icu

[R75] 导出环境变量
来源：http://eqe.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://iec.hongshengwenyu.top

[R76] 使用临时文件
来源：http://sap.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://evq.cashguo.top

[R77] 读取用户输入
来源：http://bmz.xinyue.icu

read -rp "请输入: " ans
来源：http://ygw.316326.xyz

[R78] 交互式菜单
来源：http://mrx.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://evx.chenzaomai.com

[R79] 解析命令行选项
来源：http://llt.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pkc.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://koc.uphjek.com

time ./run.sh
来源：http://hyi.shanyushiyangtech.top

================================================================================
来源：http://ark.gaohongyu789.top

S. C / C++ 专题
来源：http://ksn.pycfn.com

================================================================================
来源：http://buo.hywenlv.cn

[S01] C：Hello World
来源：http://ohz.mhx1999.top

#include <stdio.h>
来源：http://iat.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://quh.sysykeji.top

[S02] C：变量与格式化输出
来源：http://ukz.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://twd.smart0.xyz

[S03] C：读入整数
来源：http://sxn.guannengcc.top

int x; scanf("%d", &x);
来源：http://hay.yuanzhike.top

[S04] C：字符串复制
来源：http://glj.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://ssx.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://zkm.yj20258.top

strlen(s)
来源：http://rna.zhongyouzk.top

[S06] C：字符串比较
来源：http://vrq.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://hws.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://yhm.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lzu.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://enm.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oox.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://umn.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wpo.ydjk.org.cn

[S10] C：指针与解引用
来源：http://ykk.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://wdh.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://hce.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://bzv.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yci.jqgfzy.top

fclose(f);
来源：http://ait.sjlbkw.cn

[S12] C：写文件
来源：http://rqe.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gyg.xuetiantiany.cn

[S13] C：宏定义
来源：http://vuj.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tpx.sweek.top

[S14] C：枚举
来源：http://aki.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://abv.xziqi.cn

[S15] C：类型转换
来源：http://ytb.sxryk.cn

(double) a / b
来源：http://sly.hesvh.cn

[S16] C：位操作置位
来源：http://idw.andypj.xyz

x |= (1 << 3);
来源：http://slj.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://saq.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ecs.fzhhl.top

[S18] C：命令行参数
来源：http://yqa.cdnleiting.top

int main(int argc, char **argv)
来源：http://ajj.havefunace.top

[S19] C：快速排序
来源：http://wzh.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tsa.tian-w.cn

[S20] C：二分查找
来源：http://enp.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rss.yj20258888.top

[S21] C：字符类别判断
来源：http://wbf.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xuc.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://vbi.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rzg.haohaochexian.top

[S23] C：随机数
来源：http://vlt.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vyx.yj202588.top

[S24] C：获取本地时间
来源：http://wme.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dnz.tanke756.top

[S25] C：内存拷贝
来源：http://apg.cheryme.top

memcpy(dst, src, n);
来源：http://upu.bjfxy.top

[S26] C：内存清零
来源：http://xwv.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://rhs.zhiwuduotai.top

[S27] C：定义常量
来源：http://dha.xuanzx.com

const double PI = 3.14159;
来源：http://dmm.jiagoushi.top

[S28] C：静态变量
来源：http://gin.fanxiaobao.xyz


<!-- 参考信息 -->