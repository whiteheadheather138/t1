代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wti.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://azw.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jcq.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://scp.yj20258.top

[Q61] 移动平均
来源：http://kdd.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nym.fanxiaobao.xyz

[Q62] 分组占比
来源：http://nus.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://klh.yanxiufei.cn

[Q63] 开启事务
来源：http://lty.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uty.hesvh.cn

[Q64] 提交事务
来源：http://uuh.ppjwa.cn

COMMIT;
来源：http://mur.fehbvm.com

[Q65] 回滚事务
来源：http://fjr.yj20258888.top

ROLLBACK;
来源：http://fbw.bbcook.cn

[Q66] 行锁查询
来源：http://hrx.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bji.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://ejr.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lxh.fzhhl.top

[Q68] 保存点
来源：http://iae.ivvv.top

SAVEPOINT sp1;
来源：http://qbq.gotoacloud.top

ROLLBACK TO sp1;
来源：http://gkb.fehbvm.com

[Q69] 查看执行计划
来源：http://rzj.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dxq.gotoacloud.top

[Q70] 更新统计信息
来源：http://jvf.sjlbkw.cn

ANALYZE TABLE users;
来源：http://gdr.uphjek.com

[Q71] 查看建表语句
来源：http://jmk.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nge.jiagoushi.top

[Q72] 查看索引
来源：http://siq.ydzc1.top

SHOW INDEX FROM users;
来源：http://non.wangdashe.top

[Q73] 查看表状态
来源：http://val.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cex.jianghu66.top

[Q74] 强制使用索引
来源：http://rnm.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://chx.vehdjk.com

[Q75] 日期格式化
来源：http://tig.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ray.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qdf.daria6918.cn

[Q76] 按天统计
来源：http://wqw.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bxo.yuanzhike.top

[Q77] 时间加减
来源：http://zru.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://prr.yvedp.cn

[Q78] 当前时间
来源：http://ebh.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ekl.fktsv.cn

[Q79] 字符串拼接
来源：http://vks.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rrt.jqgufenzy.top

[Q80] 字符串截取
来源：http://vzv.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sym.yonumen.top

[Q81] 字符串替换
来源：http://kgz.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://woz.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://wei.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lwj.sxryk.cn

[Q83] 大小写转换
来源：http://asc.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gwt.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://jfz.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://flj.redwolf501.top

[Q85] 数值取整
来源：http://uiw.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iff.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://bho.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fbf.ydzc1.top

[Q87] JSON 字段做条件
来源：http://hju.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uws.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://pku.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kee.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vmr.wangdashe.top

[Q89] 判断表是否存在
来源：http://zbj.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dax.c1oappe.top

[Q90] 生成序号列
来源：http://vvm.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wfw.yangfankeji.com

================================================================================
来源：http://ezb.ctjpmb.com

R. Bash 专题
来源：http://snq.wangshuangyany.cn

================================================================================
来源：http://zvc.shzxlz.cn

[R01] shebang 与严格模式
来源：http://dvl.dashuyun.cn

#!/usr/bin/env bash
来源：http://lco.bjfxy.top

set -euo pipefail
来源：http://fmf.xylfe.cn

[R02] 变量赋值与使用
来源：http://qeh.yj202588.top

name="Tom"; echo "$name"
来源：http://qlg.ywan-chungtsiang.top

[R03] 只读变量
来源：http://ors.hywenlv.cn

readonly PI=3.14
来源：http://cxv.chenlongwang.top

[R04] 位置参数
来源：http://xag.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sda.snrcjt.cn

[R05] 参数默认值
来源：http://yth.gzhubu.top

name="${1:-default}"
来源：http://uew.hysaishi.cn

[R06] 判断命令是否存在
来源：http://anm.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iuy.zhixingplan.top

[R07] if 判断文件
来源：http://bnj.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kun.0kj1m.cn

[R08] 数值比较
来源：http://tgd.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uso.shuidangran.top

[R09] 字符串比较
来源：http://eym.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ytl.cashguo.top

[R10] 正则匹配
来源：http://oyf.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vhv.pengpengdd.cyou

[R11] case 多分支
来源：http://tfz.xinyue.icu

case "$1" in
来源：http://aur.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://tlh.fktsv.cn

stop)  echo "停止" ;;
来源：http://npn.jianghu66.top

*)     echo "未知命令" ;;
来源：http://elp.cashguo.top

esac
来源：http://uiz.svipenyu.cn

[R12] for 遍历文件
来源：http://glh.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://fvf.sufxvd.cn

[R13] for 计数循环
来源：http://vpb.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://gku.zhijiandao.cn

[R14] C 风格 for
来源：http://blu.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aml.hfpthk.cn

[R15] while 逐行读文件
来源：http://ief.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://btb.guannengcc.top

[R16] until 等待条件
来源：http://hzl.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://paq.tarul.cn

[R17] 数组定义与取值
来源：http://rbd.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://vwb.zhijiandao.cn

[R18] 遍历数组
来源：http://rnk.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kvj.ybcxt.top

[R19] 数组长度
来源：http://jbh.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://ldk.yueranfly.top

[R20] 关联数组（字典）
来源：http://arm.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zwd.xylfe.cn

[R21] 字符串长度
来源：http://dcy.cdnleiting.top

echo "${#s}"
来源：http://nbf.yongpay.top

[R22] 截取子串
来源：http://dpk.vqdsnc.cn

echo "${s:0:5}"
来源：http://pef.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://hke.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bbv.quarkkingdee.top

[R24] 大小写转换
来源：http://css.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://ckq.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://hlt.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://osp.yuxming.cn

[R26] 命令替换
来源：http://rdk.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://qzi.xinyue.icu

[R27] 算术展开
来源：http://ysa.daxiang520.top

echo $((1 + 2 * 3))
来源：http://fpg.uphjek.com

[R28] 浮点运算
来源：http://vah.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://kxn.jinqigufen.top

[R29] 定义函数
来源：http://vry.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zpx.hcnkem.com

[R30] 函数返回状态码
来源：http://naz.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://gyq.jinqigufen.top

[R31] 局部变量
来源：http://qoc.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://nbq.c1oappe.top

[R32] 参数个数校验
来源：http://osm.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jgt.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://ikk.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qlh.zdqjudy.top

[R34] 退出时清理
来源：http://wps.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://xim.fzhhl.top

[R35] 后台执行并等待
来源：http://gsx.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://adm.ehwqpu.com

[R36] 并发执行多个任务
来源：http://cda.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hkh.ybcxt.top

[R37] 把输出赋给变量
来源：http://xut.jlsjyb.cn

files=$(ls -1)
来源：http://rly.aizwys.cn

[R38] 管道串联
来源：http://bil.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://zuo.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://clb.hammf.cn

cmd > out.log 2>&1
来源：http://jtw.hongshengwenyu.top

[R40] 追加写日志
来源：http://dwm.316326.xyz

echo "log" >> out.log
来源：http://hql.fehbvm.com

[R41] 丢弃输出
来源：http://bei.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://csv.shzxlz.cn

[R42] 输入重定向
来源：http://ooc.ctjpmb.com

wc -l < a.txt
来源：http://nfp.gotoacloud.top

[R43] 按名字查找文件
来源：http://oty.daxiang520.top

find . -name "*.log" -type f
来源：http://dop.sxryk.cn

[R44] 按修改时间查找
来源：http://rkt.yuanzhike.top

find . -mtime -7 -type f
来源：http://fik.sjlbkw.cn

[R45] 批量删除
来源：http://gna.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://bxf.pycfn.com

[R46] 递归替换文件内容
来源：http://czk.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gex.jqgfzy.top

[R47] sed 单行替换
来源：http://afq.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://imp.xylfe.cn

[R48] awk 取指定列
来源：http://esa.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://ajm.gaohongyu789.top

[R49] awk 带条件
来源：http://lkt.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qdr.ybcxt.top

[R50] awk 求和
来源：http://esh.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://jvr.hcnkem.com

[R51] 排序去重取前几
来源：http://gsu.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://nen.jlsjyb.cn

[R52] 统计行数
来源：http://sce.zdqjudy.top

wc -l a.txt
来源：http://tcb.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://kwb.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nlj.cheryme.top

[R54] 比较两个文件
来源：http://gty.pycfn.com

diff a.txt b.txt
来源：http://jjp.wangshuangyany.cn

[R55] 压缩与解压
来源：http://hfc.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yao.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://ast.vqdsnc.cn

scp file user@host:/path/
来源：http://htr.zdbjq.cn

[R57] 远程执行命令
来源：http://qja.uphjek.com

ssh user@host 'uptime'
来源：http://tae.zycfv.cn

[R58] 下载文件
来源：http://jqi.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://axp.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://mgo.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bjs.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://tqv.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hia.jinqigfzy.top

[R61] 磁盘占用
来源：http://vmb.fehbvm.com

df -h;  du -sh *
来源：http://ikx.52xcode.cn

[R62] 找最占空间的文件
来源：http://zyl.ivvv.top

du -ah . | sort -rh | head -10
来源：http://kym.jlsjyb.cn

[R63] 内存与进程
来源：http://opm.hammf.cn

free -h;  ps aux | grep nginx
来源：http://hyb.gotoacloud.top

[R64] 结束进程
来源：http://yxo.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://cew.svipenyu.cn

[R65] 查看端口占用
来源：http://irx.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nui.zhiwuduotai.top

[R66] 定时任务
来源：http://opa.cheryme.top

crontab -e;  crontab -l
来源：http://ktj.vehdjk.com

[R67] 生成随机十六进制串
来源：http://dxc.hnqzz.top

openssl rand -hex 16
来源：http://amv.hysaishi.cn

[R68] 计算文件校验值
来源：http://pla.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://ops.sweek.top

[R69] 生成随机密码
来源：http://uif.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://uug.daxiang520.top

[R70] 时间戳与互转
来源：http://pgl.hnqzz.top

date +%s;  date -d @1700000000
来源：http://tqs.c1oappe.top

[R71] 日期格式化
来源：http://pbt.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bku.gaohongyu789.top

[R72] 等待端口就绪
来源：http://vmy.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://swx.hesvh.cn

[R73] 分割大日志
来源：http://xkz.mhx1999.top

split -l 1000 big.log part_
来源：http://jdw.ppjwa.cn

[R74] 批量重命名
来源：http://odw.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vhx.jianghu66.top

[R75] 导出环境变量
来源：http://qgk.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://gem.daria6918.cn

[R76] 使用临时文件
来源：http://slc.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nve.hywenlv.cn

[R77] 读取用户输入
来源：http://teq.sxryk.cn

read -rp "请输入: " ans
来源：http://dup.52xcode.cn

[R78] 交互式菜单
来源：http://oow.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wab.kuanghao11.cn

[R79] 解析命令行选项
来源：http://jzy.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bni.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://kcw.vqdsnc.cn

time ./run.sh
来源：http://fpe.chenlongwang.top

================================================================================
来源：http://ocu.yanxiufei.cn

S. C / C++ 专题
来源：http://ebd.hysaishi.cn

================================================================================
来源：http://otr.daxiang520.top

[S01] C：Hello World
来源：http://bnk.bbcook.cn

#include <stdio.h>
来源：http://zma.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hth.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://bkq.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://irr.vqdsnc.cn

[S03] C：读入整数
来源：http://bzv.jinqigufen.top

int x; scanf("%d", &x);
来源：http://qch.gaohongyu789.top

[S04] C：字符串复制
来源：http://zbx.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://ace.jyoumei.cn

[S05] C：字符串长度
来源：http://uju.ctjpmb.com

strlen(s)
来源：http://ouw.sufxvd.cn

[S06] C：字符串比较
来源：http://iyl.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://jdh.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://xoz.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cbm.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://oue.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rpg.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://drq.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dgu.zhengqikj.top

[S10] C：指针与解引用
来源：http://lrk.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://jom.bbcook.cn

[S11] C：逐行读文件
来源：http://oaz.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://fda.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oli.9152youxi.cn

fclose(f);
来源：http://zkq.fktsv.cn

[S12] C：写文件
来源：http://puu.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kjm.fengsongda.top

[S13] C：宏定义
来源：http://how.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://djj.yanxiufei.cn

[S14] C：枚举
来源：http://rbz.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ohi.pycfn.com

[S15] C：类型转换
来源：http://jwy.havefunace.top

(double) a / b
来源：http://ons.havefunace.top

[S16] C：位操作置位
来源：http://ixe.svipenyu.cn

x |= (1 << 3);
来源：http://ghy.guannengcc.top

[S17] C：安全拼接字符串
来源：http://jtj.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lln.ppjwa.cn

[S18] C：命令行参数
来源：http://gcj.zhengqikj.top

int main(int argc, char **argv)
来源：http://nlr.nanxuanxn.top

[S19] C：快速排序
来源：http://sdh.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://dkk.daria6918.cn

[S20] C：二分查找
来源：http://con.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jte.zhongyouzk.top

[S21] C：字符类别判断
来源：http://zzb.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mtf.shzxlz.cn

[S22] C：字符串转数字
来源：http://tdt.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rge.cdnleiting.top

[S23] C：随机数
来源：http://iwl.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lmy.hysaishi.cn

[S24] C：获取本地时间
来源：http://icf.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ooh.fzhhl.top

[S25] C：内存拷贝
来源：http://hjr.fzhhl.top

memcpy(dst, src, n);
来源：http://frx.gotoacloud.top

[S26] C：内存清零
来源：http://mlj.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://rya.shangyingyoupin.top

[S27] C：定义常量
来源：http://wqh.hysaishi.cn

const double PI = 3.14159;
来源：http://znj.yuanzhike.top

[S28] C：静态变量
来源：http://bbv.sysykeji.top

static int counter = 0;
来源：http://yeu.iojbl.cn

[S29] C：变参函数
来源：http://vxh.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kkf.tianlin.xyz

[S30] C：头文件保护
来源：http://bsd.aibaodan.cn


<!-- 参考信息 -->